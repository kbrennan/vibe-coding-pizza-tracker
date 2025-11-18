# Stream Deck Setup Guide

This guide will help you configure your Stream Deck to track pizza slices at your party using keyboard shortcuts!

## How It Works

The pizza tracker listens for keyboard number keys (1-9). Each Stream Deck button is configured to send a keyboard shortcut (like pressing "1" on your keyboard) to the browser window. When the tracker receives the keypress, it automatically decrements that pizza type and shows a visual confirmation. The change syncs instantly to all connected devices via Firebase.

**No browser windows open!** The tracker just needs to be open in a browser window in the foreground.

## Keyboard Shortcuts

| Key | Pizza Type |
|-----|------------|
| **1** | Classic Cheese |
| **2** | Margherita Pizza |
| **3** | Santorini |
| **4** | Pepperoni |
| **5** | CBR |
| **6** | Hawaiian |
| **7** | Vegan |
| **8** | Gluten-Free |
| **9** | Dairy-Free & GF |

## Stream Deck Setup Instructions

### Step 1: Add Hotkey Action

1. Open the **Stream Deck** software on your computer
2. Search for **"Hotkey"** or **"System: Hotkey"** in the actions panel
3. Drag the **Hotkey** action onto a button

### Step 2: Configure Each Button

For each pizza type you want to track:

1. **Select the button** you just created
2. Click in the **Hotkey** field
3. Press the corresponding number key (1-9) from the table above
4. **Title**: Enter the pizza name (e.g., "Cheese", "Pepperoni")
5. **Optional**: Add an icon or emoji (🍕) for visual appeal
6. Repeat for each pizza type

### Step 3: Button Layout Example

Here's a suggested 3x3 layout:

```
┌────────────┬────────────┬────────────┐
│   Cheese   │ Margherita │  Santorini │
│     🧀     │     🍅     │     🫒     │
└────────────┴────────────┴────────────┘
┌────────────┬────────────┬────────────┐
│ Pepperoni  │    CBR     │  Hawaiian  │
│     🌶️     │     🍗     │     🍍     │
└────────────┴────────────┴────────────┘
┌────────────┬────────────┬────────────┐
│   Vegan    │     GF     │   DF+GF    │
│     🌱     │   GF 🍕    │   DF+GF    │
└────────────┴────────────┴────────────┘
```

## How to Use at the Party

1. **Open the tracker**: Open https://kbrennan.github.io/vibe-coding-pizza-tracker/ in a browser window
2. **Keep window focused**: Make sure the browser window stays in focus (active window)
3. **Display on screen**: Optionally mirror/extend to a TV or projector so everyone can see
4. **Press Stream Deck buttons**: When someone takes a slice, press the corresponding button
5. **Instant feedback**: The tracker shows a visual notification and updates immediately
6. **Real-time sync**: All devices viewing the page see the update instantly via Firebase

## Important Setup Notes

### Browser Window Must Be Active
- The keyboard shortcuts only work when the browser window is **in focus** (active/foreground)
- If you switch to another app, the shortcuts won't work
- Consider dedicating a computer/tablet to run the tracker in full-screen mode

### Full-Screen Mode (Recommended)
1. Open the tracker URL
2. Press **F11** (Windows/Linux) or **Cmd+Ctrl+F** (Mac) for full-screen
3. Connect to TV/monitor for party display
4. Keep this window active while using Stream Deck

## Advanced Tips

### Multiple Displays
- Display the tracker on a TV/projector for everyone to see
- Keep the browser window active on your computer where the Stream Deck is connected
- The visual notifications will appear on all screens

### Testing Keyboard Shortcuts
- Before setting up Stream Deck, test the shortcuts manually
- Open the tracker and press number keys 1-9 on your keyboard
- You should see the slice counts decrease and notifications appear

### Multiple Stream Decks
- Set up multiple Stream Decks on different computers
- Each computer opens the tracker in a browser
- All will sync through Firebase automatically

## Troubleshooting

**Button doesn't work:**
- Make sure the browser window with the tracker is **active/in focus**
- Verify the hotkey is configured correctly (should just be the number key, no modifiers)
- Test the keyboard shortcut manually by pressing the number key

**No visual feedback:**
- Ensure the tracker webpage is loaded completely
- Check your internet connection (Firebase needs connectivity)
- Make sure you're not typing in an input field

**Count doesn't decrease:**
- Ensure the pizza has slices remaining (can't go below 0)
- Verify Firebase is initialized (wait ~2 seconds after page load)
- Check the browser console for any errors (F12)

**Stream Deck sends the number to another app:**
- The browser window must be the active window
- Click on the browser window before pressing Stream Deck buttons
- Consider using full-screen mode to prevent accidental focus loss

## Alternative: Manual Keyboard Entry

If you don't have a Stream Deck, you can simply press the number keys on your keyboard:

- Press **1** for Cheese
- Press **2** for Margherita
- Press **3** for Santorini
- And so on...

The tracker works exactly the same way!

Enjoy your party! 🍕
