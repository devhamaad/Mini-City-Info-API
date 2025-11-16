ASP.NET Core Web API – Routing Practice Project

Project Overview
This project demonstrates a well-structured ASP.NET Core Web API designed to practice and showcase routing, nested endpoint patterns, and clean DTO-based response handling.
The API models a real-world hierarchy of Cities, Places, and Attractions and focuses on producing maintainable, scalable backend code suitable for enterprise applications.

Key Features
• Structured and readable controller architecture
• RESTful endpoint design
• Nested resources (Cities → Places → Attractions)
• Route constraints for improved API reliability
• Query-parameter filtering and resource selection
• Clean DTO mapping for response consistency
• In-memory seed data for easy testing and demonstration
• Fully documented and easily extendable project structure

Project Structure
CityGuideApi/
Controllers/
CitiesController.cs
PlacesController.cs
AttractionsController.cs
Models/
City.cs
Place.cs
Attraction.cs
DTOs/
CityBasicDto.cs
CityDetailDto.cs
CitySummaryDto.cs
CityInfoDto.cs
PlaceBasicDto.cs
PlaceDetailDto.cs
AttractionBasicDto.cs
Data/
CityData.cs
Helpers/
MappingExtensions.cs
Program.cs

API Endpoints Overview

Cities
GET /api/cities
GET /api/cities/{id:int}
GET /api/cities/search?name=value
GET /api/cities/{id:int}/summary
GET /api/cities/popular
GET /api/cities/{name:alpha}/info

Places
GET /api/cities/{cityId:int}/places
GET /api/cities/{cityId:int}/places/{placeId:int}
GET /api/cities/{cityId:int}/places/search?category=value

Attractions
GET /api/cities/{cityId:int}/places/{placeId:int}/attractions
GET /api/cities/{cityId:int}/places/{placeId:int}/attractions/{id:int}
GET /api/cities/{cityId:int}/places/{placeId:int}/attractions/filter?type=value

Skills and Concepts Demonstrated
• Enterprise-level API routing organization
• Route constraints for improved error handling
• Consistent DTO-based representation models
• Nested resource navigation patterns
• LINQ for resource filtering
• Clean and maintainable backend development practices

How to Run the Project

1. Clone the repository
   git clone [https://github.com/yourusername/your-repo-name.git](https://github.com/yourusername/your-repo-name.git)

2. Open the solution in Visual Studio 2022 or Rider

3. Build and run the project
   Using CTRL + F5 or executing "dotnet run"

4. View the API through Swagger UI
   Navigate to [https://localhost:{port}/swagger](https://localhost:{port}/swagger)

Technologies Used
• ASP.NET Core Web API
• C#
• .NET 7 or .NET 8
• Swagger (OpenAPI)
• Visual Studio 2022

Screenshots
Below are recommended screenshots to include for a professional presentation:

Swagger UI – All Endpoints
[Insert Image]
[https://github.com/user-attachments/assets/7f71b9a5-950d-4589-987f-3a243d50b760](https://github.com/user-attachments/assets/7f71b9a5-950d-4589-987f-3a243d50b760)

Controllers Folder Structure
[Insert Image]
[https://github.com/user-attachments/assets/4a085146-0301-4f70-9c28-3df797e565c0](https://github.com/user-attachments/assets/4a085146-0301-4f70-9c28-3df797e565c0)

GET Cities Response Sample
[Insert Image]
[https://github.com/user-attachments/assets/687e14d9-63d5-48eb-bd18-c48a239258dc](https://github.com/user-attachments/assets/687e14d9-63d5-48eb-bd18-c48a239258dc)

Nested Attractions Endpoint
[Insert Image]
[https://github.com/user-attachments/assets/c0ed7076-8f9f-41ef-9e38-30b708ba3d96](https://github.com/user-attachments/assets/c0ed7076-8f9f-41ef-9e38-30b708ba3d96)

DTOs Overview
[Insert Image]
[https://github.com/user-attachments/assets/06596808-98ce-48ea-94c9-91edfa28ea65](https://github.com/user-attachments/assets/06596808-98ce-48ea-94c9-91edfa28ea65)

Why This Project Was Created
This project was developed to reinforce core backend engineering principles and to establish a strong foundation before transitioning into advanced topics such as EF Core, repository patterns, authentication, and production-grade API design.

Planned Enhancements
• Integration of EF Core
• Implementation of Create, Update, and Delete operations
• Addition of service and repository layers
• JWT authentication
• Pagination and sorting
• Optional React-based frontend integration
