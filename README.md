# Prayer Times Calculator

A web-based Islamic prayer times calculator that provides accurate prayer times based on your location. The calculator uses the [Adhan.js](https://github.com/batoulapps/adhan-js) library for calculations and follows various calculation methods used worldwide.


## Features

- 🕌 Accurate prayer times calculation
- 📍 Location-based automatic time calculation
- 📅 Date selection for different days
- ⚙️ Multiple calculation methods:
  - Muslim World League
  - ISNA (North America)
  - Egyptian General Authority
  - Umm Al-Qura University, Makkah
  - University of Islamic Sciences, Karachi
  - Institute of Geophysics, University of Tehran
  - Gulf Region

### Madhab Options
- Shafi (Default)
- Hanafi

### Isha End Time Calculations
- Last Third of Night
- Arabic Midnight
- Full Night (Until 1 second before Fajr)

### Additional Features
- Time adjustments for each prayer
- Start and end times for all prayers
- Precise timing with seconds
- Responsive design using Bootstrap 4
- Current prayer time highlighting
- Timezone auto-detection

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/prayer-times-calculator.git
```

2. Navigate to the project directory:
```bash
cd prayer-times-calculator
```

3. Ensure you have the following files in your assets directory:
```
assets/
├── bootstrap-4.6.2-dist/
│   ├── css/
│   │   └── bootstrap.min.css
│   └── js/
│       └── bootstrap.min.js
├── js/
│   ├── jquery.slim.min.js
│   └── popper.min.js
└── adhan-v4.4.3/
    └── lib/
        └── bundles/
            └── adhan.umd.min.js
```

4. Open `index.html` in your web browser

## Usage

1. Allow location access when prompted, or enter coordinates manually
2. Select your preferred calculation method
3. Choose your madhab (Shafi/Hanafi)
4. Select Isha end time calculation method
5. Adjust prayer times if needed (in minutes)
6. View the calculated prayer times for your location

## Dependencies

- [Adhan.js](https://github.com/batoulapps/adhan-js) - Prayer times calculation
- [Bootstrap 4.6.2](https://getbootstrap.com/docs/4.6/getting-started/introduction/) - UI framework
- [jQuery](https://jquery.com/) (slim build) - Required for Bootstrap
- [Popper.js](https://popper.js.org/) - Required for Bootstrap

## Configuration

### Prayer Time Adjustments
You can adjust the prayer times by adding or subtracting minutes:

```javascript
params.adjustments = {
    fajr: 0,
    sunrise: 0,
    dhuhr: 0,
    asr: 0,
    maghrib: 0,
    isha: 0
};
```

### Calculation Methods
Each calculation method uses different angles for Fajr and Isha:

- Muslim World League: Fajr = 18°, Isha = 17°
- ISNA: Fajr = 15°, Isha = 15°
- Egyptian: Fajr = 19.5°, Isha = 17.5°
- Karachi: Fajr = 18°, Isha = 18°
- Tehran: Fajr = 17.7°, Isha = 14°
- Gulf Region: Fajr = 18.2°, Isha = 18.2°

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- 
## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details -->

## Acknowledgments

- [Adhan.js](https://github.com/batoulapps/adhan-js) for the prayer times calculation
- Muslim World League for calculation methods
- All contributors and testers

## Support

For support, please open an issue in the GitHub repository or contact [zawad1992@gmail.com]


## TODO

- [ ] Add Qibla direction
- [ ] Add Hijri date conversion
- [ ] Add multiple language support
- [ ] Add prayer time notifications
- [ ] Add monthly prayer timetable
- [ ] Add offline support

## Notes

- Prayer times may vary slightly (1-2 minutes) from other calculators due to different calculation parameters
- The calculator takes into account timezone and DST automatically
- Height/altitude can affect prayer times slightly