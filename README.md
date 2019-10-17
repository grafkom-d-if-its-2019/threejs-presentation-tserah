# GRAFKOM THREE JS

## Komponen

### Scene (Felix)

Scene mengatur apa saja yang harus ditampilkan oleh three.js dan di mana. Scene menampung objek, pencahayaan, dan kamera

### __Camera__

Camera merupakan sebuah objek abstraksi dasar representasi kamera pada three.js. Kelas ini perlu untuk selalu diturunkan ketika akan membuat kamera baru.

Ada empat jenis tipe kamera yang disediakan secara *default*: CubeCamera, OrthographicCamera, **PerspectiveCamera**, dan StereoCamera

#### 1. Cube Camera

Membuat 6 kamera yang dirender ke WebGLRenderTargetCube

#### 2. Orthographic Camera

Kamera yang menggunakan proyeksi ortografis. Pada mode proyeksi ini, ukuran objek dalam gambar tetap konstan terlepas dari jaraknya terhadap kamera.

#### 3. Perspective Camera

Kamera yang menggunakan proyeksi perspektif.

Mode proyeksi ini dirancang untuk meniru cara mata manusia melihat. Metode ini adalah metode proyeksi yang paling umum digunakan untuk rendering 3D.

```
// var camera = new THREE.PerspectiveCamera(fov, aspect, near, far);
var camera = new THREE.PerspectiveCamera( 45, width / height, 1, 1000 );
scene.add( camera );
```

Perspective Camera memiliki beberapa atribut :

- Field of view : merupakan tingkat pemandangan yang terlihat pada layar pada saat tertentu. FOV nilainya dinyatakan dalam derajat.
- Aspect ratio : 
- Near clip
- Far clip

#### 4. Stereo Camera

Merupakan dual perspective camera yang dapat digunakan untuk efek seperti 3D Anaglyph atau Parallax Barrier.

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

```javascript
var geometry = new THREE.BoxGeometry( 1, 1, 1 );
```



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

