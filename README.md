# Extend 's  Product Protection Custom Add-on for PAS 

This add-on solves the issue where admin orders don't show offers due to some override in Pas_Core.
to install, the code has to be put in app/code/Extend, so you will end up with app/code/Extend/CustomPasPP

After copying the code, run
- bin/magento module:enable Extend_CustomPasPP

and run the magento commands
- bin/magento setup:upgrade
- bin/magento setup:di:compile
- bin/magento setup:static-content:deploy -f -j5
- bin/magento cache:clean

