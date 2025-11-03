Part 3 - Testing & Deployment (Disaster Alleviation Foundation - Web)
-------------------------------------------------------------------
Contents:
- DisasterAlleviationFoundation_Web/    <-- web app (net8.0)
- tests/                               <-- xUnit tests (net8.0)
- reports/                             <-- mock load & stress reports
- Part3_TestReport_DisasterAlleviation.docx
- azure-pipelines.yml                  <-- pipeline to build + test + publish

Run web app locally:
1. Ensure .NET 8 SDK is installed.
2. dotnet run --project DisasterAlleviationFoundation_Web
3. Open https://localhost:5001

Run tests:
1. cd tests
2. dotnet test

CI/CD:
- azure-pipelines.yml will run build and tests. Add App Service deployment task and service connection to deploy to Azure.
