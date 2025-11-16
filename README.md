╔══════════════════════════════════════════════════════════════════════╗
║              ASP.NET CORE WEB API – ROUTING PRACTICE PROJECT         ║
╚══════════════════════════════════════════════════════════════════════╝


────────────────────────────────────────────────────────────────────────
  OVERVIEW
────────────────────────────────────────────────────────────────────────
This ASP.NET Core Web API project was built to practice **Routing**,  
**Route Constraints**, **Nested Endpoints**, and **DTO Mapping** using  
realistic city → places → attractions data.

It is a read-only API using in-memory seed data to help understand  
clean controller structure and endpoint design.


────────────────────────────────────────────────────────────────────────
  FEATURES
────────────────────────────────────────────────────────────────────────
• RESTful API with clean routing  
• Nested endpoints (City → Places → Attractions)  
• Route constraints (`int`, `alpha`, ranges, etc.)  
• Query parameter filtering  
• DTO-based responses  
• In-memory data (no database required)  
• Good for learning and portfolio projects  


────────────────────────────────────────────────────────────────────────
  PROJECT STRUCTURE
────────────────────────────────────────────────────────────────────────
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
        CityInfoDto.cs
        CitySummaryDto.cs
        PlaceBasicDto.cs
        PlaceDetailDto.cs
        AttractionBasicDto.cs
    Data/
        CityData.cs
    Helpers/
        MappingExtensions.cs
    Program.cs


────────────────────────────────────────────────────────────────────────
  ENDPOINTS OVERVIEW
────────────────────────────────────────────────────────────────────────

 **Cities**
• GET /api/cities  
• GET /api/cities/{id:int}  
• GET /api/cities/search?name=Lahore  
• GET /api/cities/{id:int}/summary  
• GET /api/cities/popular  
• GET /api/cities/{name:alpha}/info  

 **Places**
• GET /api/cities/{cityId:int}/places  
• GET /api/cities/{cityId:int}/places/{placeId:int}  
• GET /api/cities/{cityId:int}/places/search?category=museum  

 **Attractions**
• GET /api/cities/{cityId:int}/places/{placeId:int}/attractions  
• GET /api/cities/{cityId:int}/places/{placeId:int}/attractions/{id:int}  
• GET /api/cities/{cityId:int}/places/{placeId:int}/attractions/filter?type=historic  


────────────────────────────────────────────────────────────────────────
  SKILLS & CONCEPTS PRACTICED
────────────────────────────────────────────────────────────────────────
• REST API design  
• Routing in ASP.NET Core  
• Route constraints  
• DTO mapping  
• Nested controller patterns  
• LINQ queries  
• Clean code structure  


────────────────────────────────────────────────────────────────────────
  HOW TO RUN THE PROJECT
────────────────────────────────────────────────────────────────────────
1. Clone the repository  
       git clone https://github.com/yourusername/your-repo-name.git

2. Open the project in Visual Studio 2022 or Rider

3. Run the API  
       Press CTRL + F5  
   or  
       dotnet run

4. Open Swagger UI  
       https://localhost:{port}/swagger


────────────────────────────────────────────────────────────────────────
  TECHNOLOGIES USED
────────────────────────────────────────────────────────────────────────
• ASP.NET Core Web API  
• C#  
• .NET 7 / .NET 8  
• Swagger (OpenAPI)  
• VS 2022 


────────────────────────────────────────────────────────────────────────
SCREENSHOTS
────────────────────────────────────────────────────────────────────────
• Screenshot of Swagger UI showing all endpoints  
![Screenshot of Swagger UI showing all endpoints](https://github.com/user-attachments/assets/7f71b9a5-950d-4589-987f-3a243d50b760)
• Screenshot of controller folder structure
![Screenshot of controller folder structure](https://github.com/user-attachments/assets/4a085146-0301-4f70-9c28-3df797e565c0)
• Screenshot of GET cities response 
![Screenshot of GET cities response ](https://github.com/user-attachments/assets/687e14d9-63d5-48eb-bd18-c48a239258dc)
• Screenshot of nested attractions endpoint
![Screenshot of nested attractions endpoint ](https://github.com/user-attachments/assets/c0ed7076-8f9f-41ef-9e38-30b708ba3d96)
• Screenshot of DTOs
![Screenshot of your DTOs](https://github.com/user-attachments/assets/06596808-98ce-48ea-94c9-91edfa28ea65)

────────────────────────────────────────────────────────────────────────
  WHY I BUILT THIS
────────────────────────────────────────────────────────────────────────
This project helped me practice real-world API design, routing patterns,  
and controller organization. It strengthened my understanding of clean  
backend architecture before moving into advanced topics like EF Core  
and repositories.


────────────────────────────────────────────────────────────────────────
  FUTURE IMPROVEMENTS
────────────────────────────────────────────────────────────────────────
• Add EF Core  
• Add Create / Update / Delete endpoints  
• Add proper repository + service layers  
• Add authentication (JWT)  
• Add pagination and sorting  
• Connect with React frontend  


╔══════════════════════════════════════════════════════════════════════╗
║                                END                                   ║
╚══════════════════════════════════════════════════════════════════════╝
