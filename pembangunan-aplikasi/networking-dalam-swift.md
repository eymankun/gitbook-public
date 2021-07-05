# Networking dalam Swift

Untuk menggunakan API, dapatkan kunci API. Boleh didapati di pembekal API.

Ada 4 langkah untuk menggunakan Networking di Swift.

1. Nyatakan dan gabungkan URL dan kunci API didalam satu string.
2. Cipta satu URLSession
3. Berikan URLSession kerja \(task\)
4. Mulakan task.

### 1. Nyatakan dan gabungkan URL 

```swift
let url = URL(string: urlString)
```

### 2. Cipta URLSession

```swift
let session = URLSession(configuration: default)
```

### 3. Berikan URLSession task

Guna URLSessionDataTask method

```swift
let task = session.URLSessionDataTask(with: url) { data, response, error } in
```

Di sini kena guna method JSONDecoder\(\). Bina satu function `parseJSON(data: Data)` untuk guna JSONDecoder.

Apabila menggunakan JSONDecoder, gunakan do try & catch.   
Contoh penggunaan: 

```swift
let decoder = JSONDecoder()
do {
     try decoder.decode(DataModel.self, form: data)
} catch {
     print(error)
}
```

### 4. Mulakan task

```swift
task.resume()
```

