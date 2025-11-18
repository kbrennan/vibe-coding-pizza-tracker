# Stream Deck Setup Guide

This guide will help you configure your Stream Deck to track pizza slices at your party!

## How It Works

Each Stream Deck button opens a special URL that automatically decrements a specific pizza type and shows a confirmation message. The change syncs instantly to all connected devices via Firebase.

## URL Format

```
https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=PIZZA_ID
```

## Pizza IDs

Use these IDs in your URLs:

| Pizza Type | ID | URL |
|------------|----|----|
| Classic Cheese | `cheese` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=cheese` |
| Margherita Pizza | `margherita` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=margherita` |
| Santorini | `santorini` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=santorini` |
| Pepperoni | `pepperoni` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=pepperoni` |
| CBR | `cbr` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=cbr` |
| Hawaiian | `hawaiian` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=hawaiian` |
| Vegan | `vegan` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=vegan` |
| Gluten-Free | `gf` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=gf` |
| Dairy-Free & GF | `df-gf` | `https://kbrennan.github.io/vibe-coding-pizza-tracker/?action=take&pizza=df-gf` |

## Stream Deck Setup Instructions

### Step 1: Add Website Action

1. Open the **Stream Deck** software on your computer
2. Drag the **Website** action onto a button
3. Or search for "Website" in the actions panel and drag it to your Stream Deck

### Step 2: Configure Each Button

For each pizza type you want to track:

1. **Select the button** you just created
2. In the **URL** field, paste the corresponding URL from the table above
3. **Title**: Enter the pizza name (e.g., "Cheese", "Pepperoni")
4. **Optional**: Add an icon or emoji (🍕) for visual appeal
5. Repeat for each pizza type

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

1. **Display the tracker**: Open https://kbrennan.github.io/vibe-coding-pizza-tracker/ on a TV or monitor
2. **Hand out slices**: When someone takes a slice, press the corresponding Stream Deck button
3. **Instant feedback**: The tracker updates immediately and shows a confirmation message
4. **Real-time sync**: All devices viewing the page see the update instantly

## Advanced Tips

### Custom Browser
- By default, Stream Deck opens URLs in your default browser
- You can configure it to use a specific browser in Stream Deck settings

### Multiple Stream Decks
- Set up multiple Stream Decks around the pizza table
- All will sync through Firebase automatically

### Testing
- Before the party, test each button to make sure URLs work correctly
- You can reset counts using the red "Reset All Counts" button on the web page

### Visual Display
- Consider keeping the tracker open in full-screen mode on a large display
- The animated notification will appear when buttons are pressed

## Troubleshooting

**Button doesn't work:**
- Check the URL is copied correctly
- Make sure there are no extra spaces
- Verify the pizza ID matches exactly (case-sensitive)

**No visual feedback:**
- Make sure you're viewing the page when pressing the button
- Check your internet connection (Firebase needs connectivity)

**Count doesn't decrease:**
- Ensure the pizza has slices remaining (can't go below 0)
- Verify Firebase is initialized (wait ~2 seconds after page load)

## Alternative: QR Codes

If you don't have a Stream Deck, you can create QR codes for each URL:

1. Use a QR code generator: https://www.qr-code-generator.com/
2. Generate a QR code for each pizza URL
3. Print and place them near the pizza boxes
4. People scan with their phones to register their slice choice

Enjoy your party! 🍕
