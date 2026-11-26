# DLSP: Checking usage and getting connected

**Presenter:** Mohammadhossein Zare  
**Week and topic:** 10 / 01  
**Presentation:** [PowerMD source](presentation.md) · [Slides (.pptx)](DLSP-Presentation.pptx)

## The design decision

DLSP separates monitoring a mobile VPN subscription from the work of setting up or managing it. **Status** shows data, time and validity. **Manage** groups connection and service actions. This keeps different goals from competing in one view.

## Example

To connect a second device, open Manage and choose **Get config** for a setup configuration or **Subscription link** for a link the app can use. **Add traffic** and **Add time** are separate upgrade actions. The [prototype](https://www.figma.com/proto/xlMfwAFsziZRuoTJ4dYbMb?node-id=5-2) uses demonstration values.

## Evidence and takeaway

The two implemented views document the separation. Live users gave positive informal feedback. The feedback was not a measured comparison. The takeaway is to group actions by user intent, with less scrolling as an additional benefit.
