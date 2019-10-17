# GRAFKOM THREE JS

## Komponen

### Scene (Felix)

Scene mengatur apa saja yang harus ditampilkan oleh three.js dan di mana. Scene menampung objek, pencahayaan, dan kamera

### Camera (Lia)

Camera merupakan sebuah objek abstraksi representasi kamera. Ada empat jenis tipe kamera yang disediakan secara *default*: CubeCamera, OrthographicCamera, **PerspectiveCamera**, StereoCamera

#### Perspective Camera

Atribut

- Field of view
- Aspect ratio
- Near clip
- Far clip

### Geometri (Setya)

Geometri merupakan sebuah representasi objek 3D yang didefinisikan oleh beberapa `THREE.Vector3` atau `THREE.Color`

```javascript
var geometry = new THREE.Geometry();

geometry.vertices.push(
	new THREE.Vector3( -10,  10, 0 ),
	new THREE.Vector3( -10, -10, 0 ),
	new THREE.Vector3(  10, -10, 0 )
);
```

Terdapat beberapa geometri yang sudah *predefined* oleh three.js:

- `THREE.BoxGeometry`
- `THREE.CircleGeometry`
- `THREE.ConeGeometry`
- `THREE.DodecahedronGeometry`
- `THREE.TorusGeometry`
- `THREE.TubeGeometry`
- `THREE.ShereGeometry`

dan lain-lain. Masing-masing turunan dari `THREE.Geometry` di atas memiliki constructor dengan parameter yang berbeda.

### Material (Bagas)

Material merupakan sebuah class abstract yang mendeskripsikan tampilan sebuah objek.

Contoh Material yang sudah ada di three.js

- `THREE.MeshBasicMaterial`
- `THREE.ShaderMaterial`
- `THREE.RawShader`

```javascript
var material = new THREE.MeshBasicMaterial( { color: 0x00ff00 } );
```



### Mesh (felix)

Deskripsi mesh

## Implementasi

### Rendering (reza)

yang ada requestanimationframe

### Transformasi (reza)

Termasuk yang ada rotation dll2



https://threejs.org/docs/index.html#manual/en/introduction/Creating-a-scene



**jangan lupa lihat panel sebelah kiri, itu ada resource banyak**

