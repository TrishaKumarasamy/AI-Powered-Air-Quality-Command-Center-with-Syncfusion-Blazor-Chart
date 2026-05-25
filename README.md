# Air Quality Chart Tracker

An AI-powered air quality monitoring dashboard built with Blazor and Charts. This application leverages Azure OpenAI to generate intelligent air pollution predictions, providing real-time insights and forecasts for any location worldwide.

## Overview

Air Quality Chart Tracker is a modern web application that combines interactive data visualization with AI-driven predictive analytics. Users can search for any location, view current pollution metrics, analyze 7-day trends, and generate AI-powered forecasts for the next 30 days. The application features an intuitive dashboard layout with real-time data updates and interactive geographical mapping.

### Features

- **AI-Powered Predictions**: Leverage Azure OpenAI to generate realistic air quality forecasts based on historical trends
- **Interactive Charts**: Visualize pollution data with Charts for better insights
- **Location Search**: Search air quality data for any location worldwide
- **Predictive Analytics**: Generate 30-day air quality forecasts using machine learning models
- **Real-time Metrics**: Track current pollution index, 7-day averages, and air quality status
- **Geographical Mapping**: View location data on interactive maps with markers
- **Responsive Dashboard**: Adaptive layout that works seamlessly on different screen sizes

## Architecture

The application is built with a modern, scalable architecture:

- **Frontend**: Blazor with interactive server-side rendering
- **Visualization**: Blazor components for charts and maps
- **AI/ML**: Azure OpenAI for intelligent pollution forecasting
- **Data Management**: JSON-based data storage with fallback mechanisms

### Configure Azure OpenAI

Before running the application, you need to set up Azure OpenAI credentials:

1. Open `appsettings.json`
2. Update the Azure OpenAI configuration:

```json
{
  "AzureOpenAI": {
    "Endpoint": "https://your-resource.openai.azure.com/",
    "ApiKey": "your-api-key",
    "DeploymentId": "your-deployment-model-name"
  }
}
```

> [!NOTE]
> For local development, you can also use `appsettings.Development.json` to override these settings.

## Prerequisites

- [.NET SDK 8.0](https://dotnet.microsoft.com/download/dotnet/8.0) or later
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later
- [Visual Studio Code](https://code.visualstudio.com/)

## Getting Started

### Clone the repository

```bash
git clone https://github.com/SyncfusionExamples/AI-Powered-Air-Quality-Command-Center-with-Syncfusion-Blazor-Chart.git
cd AI-Powered-Air-Quality-Command-Center-with-Syncfusion-Blazor-Chart
```

### Run with Visual Studio

1. Open the solution file using Visual Studio 2022 or later.
2. Restore the NuGet packages by rebuilding the solution.
3. Build the project to ensure there are no compilation errors.
4. Run the project.

### Run with .NET CLI

```bash
# Restore dependencies
dotnet restore

# Run the project
dotnet run
```

## Resources

- [Microsoft Blazor Documentation](https://learn.microsoft.com/en-us/aspnet/core/blazor/)
- [Azure OpenAI Documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/reference)
- [Azure Identity Documentation](https://learn.microsoft.com/en-us/dotnet/api/overview/azure/identity-readme)
