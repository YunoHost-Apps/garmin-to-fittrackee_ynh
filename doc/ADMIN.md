After installation, you have to perform following commands to be able to use Garmin-to-FitTrackee.

``yunohost app shell __APP__``
``env HOME=__INSTALL_DIR__ __INSTALL_DIR__/venv/bin/garmin2fittrackee setup garmin --email "__GARMIN_EMAIL__" --password "__GARMIN_PASSWORD__" --store``

After following command, an URL will be shown. Open this URL in a browser, login to your FitTrackee account. After the operation, you will have to copy the link and put it back in the terminal (something like ``https://localhost/...``).

``env HOME=__INSTALL_DIR__ __INSTALL_DIR__/venv/bin/garmin2fittrackee setup fittrackee --client-id __FITTRACKEE_ID__ --client-secret __FITTRACKEE_SECRET__ --fittrackee-domain __FITTRACKEE_DOMAIN__ --force``

``env HOME=__INSTALL_DIR__ __INSTALL_DIR__/venv/bin/garmin2fittrackee sync``

Now, __APP__ will sync every hour o’clock.
