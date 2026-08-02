# yesmeta.xyz

A satirical take on chat etiquette. Unlike the traditional *nometa* concept that discourages meta-questions, this site jokingly advocates for asking them to ensure "polite" communication.

## 🌍 Internationalization

The site supports multiple languages:
- **English** (`index.html` - default)
- **Russian** (`ru.html`)
- **Ukrainian** (`uk.html`)
- **Uzbek** (`uz.html`)

## 🚀 Features

- **Lightweight**: Pure HTML and CSS. Zero JavaScript dependencies.
- **Optimized Delivery**: Configured with a production-ready `Caddyfile`.
- **Security Headers**: Built-in strict transport security, content-type options, and frame options.
- **Caching**: Configured for aggressive caching of static assets.

## 📂 Project Structure

```text
├── index.html   # Main English page
├── ru.html      # Russian translation
├── uk.html      # Ukrainian translation
├── uz.html      # Uzbek translation
├── style.css    # Shared stylesheet
├── Caddyfile    # Caddy web server configuration
└── README.md    # Project documentation
```

## 🛠 Local Development

To run the project locally, you can use any static file server. 

**Using Python:**
```bash
python3 -m http.server 8080
```
Then visit `http://localhost:8080`.

**Using Node.js (http-server):**
```bash
npx http-server . -p 8080
```

## 🌐 Deployment (Caddy)

This repository includes a `Caddyfile` for seamless deployment with [Caddy Server](https://caddyserver.com/), which automatically provides HTTPS.

1. Clone the repository to your server (default path in config is `/opt/yesmeta`).
2. Make sure your domain's DNS `A`/`AAAA` records point to your server.
3. Start or reload Caddy using the included configuration:
   ```bash
   caddy reload --config /opt/yesmeta/Caddyfile
   ```
