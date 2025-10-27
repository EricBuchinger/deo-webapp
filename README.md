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
