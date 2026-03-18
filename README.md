<img src="https://socialify.git.ci/dlozilab/c--simple-server/image?language=1&owner=1&name=1&stargazers=1&theme=Light" alt="c--simple-server" width="640" height="320" />

# c#-simple-server

A lightweight, high-performance web server built with C# and .NET 10. Designed for those who love the simplicity of Express.js but need the power and type-safety of the .NET ecosystem.

## 🚀 Quick Start

### Prerequisites
* **.NET 10 SDK** (The core runtime and CLI)
* **Git**

### Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/dlozilab/c--simple-server.git
   cd c--simple-server
   ```

2. **Restore dependencies**
   *Unlike npm install, this happens automatically on build, but you can run it manually:*
   ```bash
   dotnet restore
   ```

3. **Run the server**
   ```bash
   dotnet run
   ```
   The server will start by default at `http://localhost:5000`.

## 🛠 Features
- **Minimal API:** No controllers, no boilerplate, just routes.
- **Top-Level Statements:** Single-file entry point (Program.cs).
- **Environment Aware:** Uses `appsettings.json` for config and supports Secret Manager for local dev.

## 📖 How to add a route
Open `Program.cs` and add your logic just like Express:

```csharp
app.MapGet("/hello", () => new { Message = "Hello World" });
```

## 🔒 Security Note
This project uses a `.gitignore` specifically tuned for .NET. 
- `bin/` and `obj/` are ignored.
- `appsettings.Development.json` is ignored to prevent accidental credential leaks.
- Use `dotnet user-secrets` for local sensitive data.


