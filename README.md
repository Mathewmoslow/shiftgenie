# ShiftGenie 🍽️

A simple, intuitive web app for servers to track their shifts and calculate income to meet monthly expense goals.

## Features

- **Visual Calendar Interface**: Click days to select/deselect shifts
- **Income Tracking**: Automatic calculation based on typical dinner shift earnings
- **Goal Progress**: Real-time progress bar showing how close you are to your monthly target
- **Smart Recommendations**: Suggests which shifts to pick up to meet your goals
- **Responsive Design**: Works on desktop, tablet, and mobile

## Default Shift Estimates (Dinner 4pm-12am)

Based on industry research for typical dinner shift earnings:
- **Monday**: $70 (slowest night)
- **Tuesday**: $80
- **Wednesday**: $90
- **Thursday**: $100
- **Friday**: $180 (weekend rush)
- **Saturday**: $200 (busiest night)
- **Sunday**: $120

## How to Use

1. Enter your monthly expense target (default: $4000)
2. Set the current day of the month for planning purposes
3. Click on calendar days to select your scheduled shifts
4. Green days = selected shifts
5. View your projected income and remaining amount needed
6. Check the suggestions panel for recommended additional shifts

## Customizing Shift Values

To update the shift income values, edit the `shiftIncomes` object in the JavaScript:

```javascript
const shiftIncomes = {
    0: 120,  // Sunday
    1: 70,   // Monday
    2: 80,   // Tuesday
    3: 90,   // Wednesday
    4: 100,  // Thursday
    5: 180,  // Friday
    6: 200   // Saturday
};
```

## Deployment

This app is deployed via GitHub Pages at: https://mathewmoslow.github.io/shiftgenie/

## License

MIT
