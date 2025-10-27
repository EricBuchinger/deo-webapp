# DevOps Tutorial – deo-webapp  

Dieses Repository enthält die Web-Applikation **„Deo WebApp“** als Teil eines **DevOps Tutorials**.  
Es zeigt Beispiele für moderne Entwicklung mit . NET, Frontend, Tests, CI/CD, Containerisierung und Infrastruktur-Architektur.

---

## 📂 Inhalte  

- `Deo.Backend/` – Backend-Applikation (z. B. in C# / ASP.NET)  
- `Deo.Frontend/` – Frontend-Applikation (z. B. HTML/CSS/JS)  
- `Deo.WebApp.sln` – Solution-Datei für das gesamte Projekt  
- `compose.yaml` – Docker Compose-Definition für lokale Entwicklung  
- `kubernetis_commands.txt` – Beispiel-Kommandos für Kubernetes-Deployments  
- `prometheus.yml` – Konfiguration für Monitoring via Prometheus  
- `terraform_commands.txt` – Beispiel-Kommandos zur Infrastruktur-Provisionierung via Terraform  
- Tests: `Deo.Backend.Tests/`, `Deo.Frontend.Tests/`, `Deo.WebApp.Tests/`

---

## 🎯 Zielsetzung  

Das Projekt verfolgt folgende Ziele:  

- Demonstration einer Full-Stack-WebApp mit getrenntem Backend und Frontend  
- Integration von automatisierten Tests auf allen Ebenen  
- Containerisierung & Orchestrierung (Docker, Kubernetes)  
- Infrastruktur als Code (Terraform)  
- Monitoring & Observability (Prometheus)  
- CI/CD – automatisierte Builds, Tests, Deployments  
- DevOps Best Practices in einem realistischen Beispiel  

---

## ⚙️ Voraussetzungen  

Damit du das Projekt lokal zum Laufen bringen kannst, brauchst du:  

- [.NET SDK](https://dotnet.microsoft.com/) (z. B. Version 7 oder höher)  
- Node.js / npm (falls Frontend mit Node betrieben wird)  
- Docker & Docker Compose  
- Optional: Kubernetes-Cluster (minikube, kind, k3s)  
- Optional: Terraform CLI  
- Git-Client  

---

## 🚀 Installation & Lokales Setup  

1. **Repository klonen:**  
   ```bash
   git clone https://github.com/EricBuchinger/deo-webapp.git
   cd deo-webapp

2. **.NET-Solution öffnen oder über CLI builden:**
```bash
dotnet restore
dotnet build
```


3. **Docker Compose starten (aus dem Projektroot):**

`docker compose up --build`

→ Das setzt Backend, Frontend und ggf. Datenbanken in Containern auf.

4. **Frontend im Browser öffnen:**

Standardmäßig unter http://localhost:3000

5.**Tests ausführen:**

dotnet test ./Deo.Backend.Tests
dotnet test ./Deo.Frontend.Tests
dotnet test ./Deo.WebApp.Tests

## ☁️ Deployment & Infrastruktur

Docker Compose – Lokale Services (compose.yaml).

Kubernetes – Beispiel-Kommandos in kubernetis_commands.txt.

Terraform – Infrastruktur-Provisionierung über terraform_commands.txt.

Monitoring – prometheus.yml für Prometheus-Konfiguration.

## 🧩 Architekturübersicht

Backend: REST-API / GraphQL (C#, ASP.NET Core).

Frontend: Moderne WebApp mit HTML/CSS/JavaScript oder Framework (z. B. React).

Containerisierung: Jede Komponente läuft in einem separaten Docker-Container.

Orchestrierung: Deployment über Kubernetes.

Infrastructure as Code: Terraform für Cloud-Ressourcen.

Monitoring: Prometheus sammelt Metriken (optional Grafana).

CI/CD: GitHub Actions für Build, Test & Deployment.

## 🔄 CI/CD Workflow

Build: Prüft Code-Qualität, kompiliert Backend & Frontend.

Test: Führt Unit- und Integrationstests aus.

Container-Build: Erzeugt Docker-Images.

Deployment: Automatisch in Staging oder Produktion (je nach Branch).
