# Scaler 2 Multi-Out Routing in Ableton

This is a custom template based on the template provided [here](https://forum.scalerplugin.com/t/scaler-2-7-multi-out-template-for-ableton/11970/2).

This template provides multi out support for Scaler 2 within Ableton, using the MacOS IAC MIDI Driver.

You can drop the template into your `User Library/Templates` and either open it as a new project, or expand it and drop the `Scaler` group into your existing projects.

## MacOS IAC Driver for MIDI Routing

[Documentation](https://support.apple.com/guide/audio-midi-setup/transfer-midi-information-between-apps-ams1013/mac) copied from Apple.

### Transfer MIDI information between apps in Audio MIDI Setup on Mac

In Audio MIDI Setup, use the IAC Driver to let MIDI apps transfer information to each other. For example, you might have a MIDI keyboard app send its MIDI data to a MIDI synthesizer app.

To allow MIDI apps to transfer information, you need to set up at least one bus (sometimes referred to as a port) in the IAC Driver. One app uses the bus as a destination to send information, and another app uses it as a source, to receive information.

1. In the Audio MIDI Setup app on your Mac, choose Window > Show MIDI Studio.

2. In the MIDI Studio window, double-click the IAC Driver.

3. In the Properties window, select “Device is online” to turn on the driver.

4. To set up the ports, do any of the following:

   - By default, “Bus 1” should already exist if this is your first time configuring it - _use this as the default_
   - Add a bus: Click the Add button below the list of ports.
   - Rename a bus: Double-click the bus in the list, enter the new name, then press the Return key.
   - Remove a bus: Select the bus in the list, then click the Remove button .

5. Select the bus you want to use to transfer information, then specify the number of MIDI In and MIDI Out connectors.

6. Click Apply.

### Ableton Configuration

1. Open Preferences, goto MIDI
2. Enable Track on “In: IAC Driver (Bus 1)”
3. Enable Track on “Out: IAC Driver (Bus 1)”

\*\* If you setup a custom Bus, or renamed the default Bus, enable Track on the In/Out for that specific Bus.
