# AlertDialogExample

```java
private void showDialog(){
    AlertDialog.Builder alertDialogBuilder = new AlertDialog.Builder(this);

    alertDialogBuilder.setTitle("Keluar dari aplikasi?");

    alertDialogBuilder
            .setMessage("Klik Ya untuk keluar!")
            .setIcon(R.mipmap.ic_launcher)
            .setCancelable(false)
            .setPositiveButton("Ya",new DialogInterface.OnClickListener() {
                public void onClick(DialogInterface dialog,int id) {
                    Toast.makeText(getApplicationContext(), "Ya", Toast.LENGTH_SHORT).show();
                }
            })
            .setNegativeButton("Tidak",new DialogInterface.OnClickListener() {
                public void onClick(DialogInterface dialog, int id) {
                    Toast.makeText(getApplicationContext(), "Tidak", Toast.LENGTH_SHORT).show();
                }
            });

    AlertDialog alertDialog = alertDialogBuilder.create();

    alertDialog.show();
}
```

---

```
Copyright 2022 M. Fadli Zein
```