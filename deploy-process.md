# Dashboardable-Reports Deployment

The deployment process for dashboardable-reports is similar to the process for traditional base reports. There are a few key differences, outlined below.

## Package Format

The package for a dashboardable report has the same structure as a base report.

{img001}

The primary difference is found in the report.properties file. Here we add two new properties:

{img002}

 1. ```Dashboardable="Y"```

	This property marks the report as dashboardable. It will be discoverable in *My Report Profiles* when you select the 'Dashboardable' radio button.

 2. ```Server\_URL="/public/Dashboards/myPackageName"```

	This is the path to the report on JasperReports Server. The deployment process automatically uploads the dashboard to the default directory, ```/public/Dashboards```. The server URL must point to a dashboard under this directory.

## Deployment

The usual process for deploying reports applies here.

1. Create an archive of the package's files.

2. Upload the archive to *Jasper Custom Reports.*

3. Distribute the dashboard to users.
