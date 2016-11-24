
## Validar Conexión a internet

```
 public static boolean isConnectingToInternet(Context context) {

    ConnectivityManager cm =
            (ConnectivityManager) context.getSystemService(Context.CONNECTIVITY_SERVICE);

    NetworkInfo activeNetwork = cm.getActiveNetworkInfo();

    return activeNetwork != null &&
            activeNetwork.isConnectedOrConnecting();
}
```

Permisos :
```
  <uses-permission android:name="android.permission.INTERNET" /> 
  <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" /> 
```
