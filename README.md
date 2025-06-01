## 🌀 **Fast `curl` Command**

### 📥 **Basic Usage**

```bash
curl https://example.com
```

* Fetches the HTML content of the page.

---

### 📤 **Download File**

```bash
curl -O https://example.com/file.zip
```

* Saves file with original name (`-O` = remote filename).

```bash
curl -o myfile.zip https://example.com/file.zip
```

* Saves as `myfile.zip` (`-o` = output filename).

---

### 🔐 **HTTPS with Insecure Certificate**

```bash
curl -k https://example.com
```

* Skips SSL certificate validation (use cautiously).

---

### 📬 **Send GET Request with Parameters**

```bash
curl "https://example.com/api?name=John&age=30"
```

---

### ✍️ **Send POST Request**

```bash
curl -X POST -d "name=John&age=30" https://example.com/api
```

* `-d` sends form data.

---

### 📦 **Send JSON Data**

```bash
curl -X POST -H "Content-Type: application/json" \
     -d '{"name":"John","age":30}' \
     https://example.com/api
```

---

### 🧾 **Include Headers**

```bash
curl -H "Authorization: Bearer TOKEN" https://example.com/api
```

---

### 📄 **Save Output to File**

```bash
curl https://example.com -o page.html
```

---

### 📂 **Upload File**

```bash
curl -F "file=@/path/to/file.jpg" https://example.com/upload
```

* `-F` simulates a file upload (like from an HTML form).

---

### 📊 **Show Response Headers**

```bash
curl -I https://example.com
```

---

### 🚦 **Follow Redirects**

```bash
curl -L https://bit.ly/some-short-link
```

---

### 🐾 **Verbose Mode (Debug)**

```bash
curl -v https://example.com
```
