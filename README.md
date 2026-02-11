# Spark Skeleton

Spark Skeleton brings modern development conventions to the Spark Java framework. Built on top of Spark, it adds annotation-based routing, fluent database migrations, middleware system, CSRF protection, authentication, and more — all while keeping the simplicity of a micro-framework.

## 🎯 Why this project?

Spark Java is an excellent micro-framework, but it lacks modern conventions. This boilerplate fills the gap by adding:

- **Routing annotations** — no more manually declared routes
- **Middleware system** — `@Before` and `@After` annotations with built-in middlewares
- **Fluent migrations** — Laravel-inspired database migrations
- **Security & Auth** — UserDetailsService abstraction with role-based access control
- **CSRF protection** — annotation-based CSRF validation
- **Repository pattern** — automatic dependency injection
- **Template engine** — Pebble integrated directly into controllers
- **Flash messages** — temporary notifications without external dependencies

## ✨ Main Features

| Feature | Description |
|---------|-------------|
| 🛣️ **Annotation-based routing** | `@GET`, `@POST`, `@PUT`, `@DELETE`, `@PATCH` on your methods |
| 🔒 **Middleware system** | `@Before` / `@After` with built-in CORS, rate limiting, logging, API keys |
| 🗃️ **Fluent migrations** | `table.string("title").notNull()` instead of raw SQL |
| 🔐 **Security & Auth** | `UserDetailsService` + `@HasRole` for role-based protection |
| 🛡️ **CSRF Protection** | `@CsrfProtect` annotation with automatic token validation |
| 💉 **Dependency Injection** | Automatically injects your `@Repository` into controllers |
| 📦 **ActiveRecord models** | ActiveJDBC with getters/setters to manipulate your models cleanly |
| 🎨 **Integrated templating** | `render("view.html", data)` directly in your controllers |
| 💬 **Flash messages** | `redirectWithFlash()` for temporary notifications |
| 🐛 **Custom Error Handler** | Detailed stack traces in dev, clean pages in production |

## 🚀 Quick Start

```bash
git clone https://github.com/kainovaii/spark-skeleton.git
cd spark-skeleton
./build.bat
```

→ The app runs on `http://localhost:8888`

## 📦 Tech Stack

- **Spark Java** - Web micro-framework
- **ActiveJDBC** - Lightweight ORM with ActiveRecord pattern
- **Pebble** - Modern template engine
- **Maven** - Build & dependency management

## 📖 Documentation

Full documentation is available at `https://spark.kainovaii.dev`.

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

## 📝 License

[MIT](LICENSE)