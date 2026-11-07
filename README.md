# TRADER R AI — Flutter starter

This is the first UI prototype for an educational trading-analysis app.

## Included
- Dark black and gold app theme
- Home dashboard
- Analyzer screen with market/timeframe selectors and a sample analysis state
- Academy learning-path screen
- Trading journal placeholder
- Bottom navigation

## Not included yet
- Real AI chart-image analysis
- Live market prices or economic calendar
- User accounts, cloud journal storage, or notifications
- APK build/signing

The sample analysis is explicitly a placeholder, not a market signal.

## Run locally
1. Install Flutter SDK and Android Studio.
2. Extract this folder.
3. In this folder run:
   ```bash
   flutter pub get
   flutter run
   ```
4. To build an APK after testing:
   ```bash
   flutter build apk --release
   ```
   APK output is normally at `build/app/outputs/flutter-apk/app-release.apk`.

## Next engineering steps
1. Add chart image selection and upload.
2. Add a secure backend endpoint for AI vision analysis. Keep API keys on the server; never ship secret keys in the app.
3. Add trusted market-data and economic-calendar providers.
4. Add journal persistence and privacy controls.
5. Test analysis against labeled historical examples before presenting outputs as useful.

## Safety design
The app is for education and chart interpretation. It must not promise profits, claim certainty, or automatically execute trades. It should show uncertainty and say "insufficient evidence" when the chart cannot support a conclusion.
