# godot-iap-template
IAP implementation based on Godot 2 docs.

1. Add "iap.gd" to Autoloads. See Project > Project Settings > AutoLoad

2. To enable Godot IAP module

- Project > Project Settings
- write [Category : "android"] | [Property : "modules"] | [Type : "String"] and click "Add"
- Click "Android" on left panel
- Double click on right filed of "modules"
- write "org/godotengine/godot/GodotPaymentV3"

3. To test in-app purchase on android device

- Add "com.android.vending.BILLING\" permission at Project > Export > Android > User Permissions > custom_permissions=PoolStringArray( "com.android.vending.BILLING" )
- Export APK and upload it as alpha or beta stage to Google Play Developer Console and publish it.
- There should be activated in-app item at Play Store
