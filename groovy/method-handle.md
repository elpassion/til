# `.&` Method handle

Instead of using anonymous classes or closures, you may use method handle by prefixing method with `&`.

```groovy
void onCreate(Bundle savedInstanceState) {
    // ...
    loginButton.onClickListener = this.&onLoginButtonClick
}

private void onLoginButtonClick(View view) {
    // ...
}
```

where `onClickListener` expects [`View.OnClickListener`] interface.

[`View.OnClickListener`]: http://developer.android.com/reference/android/view/View.OnClickListener.html
