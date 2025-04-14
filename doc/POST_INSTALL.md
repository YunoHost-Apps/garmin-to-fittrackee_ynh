After installation, you have to perform following commands to be able to use Garmin-to-FitTrackee.

__INSTALL_DIR__/venv/bin/garmin2fittrackee setup config-tool --database-path __INSTALL_DIR__

After following command, an URL will be shown. Open this URL in a browser, login to Garmin Connect. After the operation, you will have to copy the link and put it back in the terminal.
__INSTALL_DIR__/venv/bin/garmin2fittrackee setup garmin --email "$garmin_email" --password "$garmin_password" --store

__INSTALL_DIR__/venv/bin/garmin2fittrackee setup fittrackee --client-id "$fittrackee_id" --client-secret "$fittrackee_secret" --fittrackee-domain "$fittrackee_domain" --force

__INSTALL_DIR__/venv/bin/garmin2fittrackee sync