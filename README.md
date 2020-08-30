# tailwind-toast-notification
toast notification yang dibuat menggunakan tailwind dan javascript untuk menampilkannya

## Dokumentasi

##### inisiasi function
```javascript
TToast(message, mode, costumize);
```
### Parameters

##### message : String

##### mode : String
```javascript
'success', 'info', 'warning', 'danger'
  
default = 'success'
```

##### costumize : Object
```
- iconSize : String | default = '1.8em'
- roundedClass : String | default = tidak ada
- textClass : String | default = tidak ada
- duration : Numbers | default = 3000 (3detik)
- animation : String | default = tidak ada
```
saya menyarankan untuk menggunakan em untuk iconSize.  
pada textClass berisi style yang akan diberikan untuk text pada toast notification.  
roundedClass & textClass berisi class yang diberikan oleh tailwindcss.  
untuk menggunakan animation, harus mengincludekan ttoast.css terlebih dahulu.  

### Animation class
```
'rotate','flick','zoomin','opacity'
```

### Example
```javascript
  success
  TToast('pesan sukses','success', {roundedClass: 'rounded', textClass: 'font-bold cursor-default', duration: 3000, animation: 'rotate'})
  
  info
  TToast('pesan info','info', {roundedClass: 'rounded', textClass: 'font-semibold cursor-pointer', duration: 5000, animation: 'flick'})
  
  warnning
  TToast('pesan warning','warning', {roundedClass: 'rounded', textClass: 'underline text-gray-900 cursor-default', duration: 2500, animation: 'zoomin'})
  
  danger
  TToast('pesan danger','danger', {roundedClass: 'rounded', textClass: 'text-xl', duration: 3000, animation: 'opacity'})
```

### DEMO
[https://hudadamar21.github.io/tailwind-toast-notification](https://hudadamar21.github.io/tailwind-toast-notification)

### Tutorial
null

