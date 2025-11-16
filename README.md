<div align="center">
  <h1 style="margin-bottom: 0;">City–Places–Attractions API</h1>
  <p style="font-size: 16px; color: #555;">
    A clean, structured ASP.NET Core Web API demonstrating nested routing, DTO mapping, and REST best practices.
  </p>
</div>

<br/>

<div style="display: flex; flex-direction: column; gap: 20px;">

  <h2 style="color: #333;">📌 Project Overview</h2>
  <p style="line-height: 1.6; color: #444;">
    This project showcases a multi-level routing structure (<strong>City → Place → Attraction</strong>) 
    implemented in ASP.NET Core Web API.  
    It focuses on clean architecture, DTO-driven responses, in-memory data handling, and route constraints.
  </p>

  <h2 style="color: #333;">🚀 Features</h2>
  <ul style="line-height: 1.8; color: #444;">
    <li>RESTful API design</li>
    <li>Nested routes with <code>cityId</code>, <code>placeId</code>, and <code>attractionId</code></li>
    <li>DTO-based response shaping</li>
    <li>Filtering endpoint (e.g., filter attractions by type)</li>
    <li>In-memory seeded data</li>
    <li>Swagger documentation enabled</li>
  </ul>

  <h2 style="color: #333;">🛠 Tech Stack</h2>
  <ul style="line-height: 1.8; color: #444;">
    <li>ASP.NET Core Web API</li>
    <li>C#</li>
    <li>Swagger / Swashbuckle</li>
  </ul>

  <h2 style="color: #333;">📁 Project Structure</h2>
  <pre style="background: #f4f4f4; padding: 15px; border-radius: 8px;">
/Controllers
   CitiesController.cs
/Models
   City.cs
   Place.cs
   Attraction.cs
/DTOs
   CityBasicDto.cs
   PlaceBasicDto.cs
   AttractionBasicDto.cs
/Data
   CityData.cs
  </pre>

  <br/>

 <h2 style="color: #333;">🖼 Screenshots</h2>

  <p style="color:#777;">Add your images by replacing the <em>src</em> URLs.</p>

  <div style="margin-bottom: 20px;">
    <strong>Swagger UI – All Endpoints</strong><br/>
    <img src="" alt="Swagger Screenshot" style="max-width: 100%; border-radius: 8px; margin-top: 10px;" />
  </div>

  <div style="margin-bottom: 20px;">
    <strong>Controller Folder Structure</strong><br/>
    <img src="" alt="Controller Folder Screenshot" style="max-width: 100%; border-radius: 8px; margin-top: 10px;" />
  </div>

  <div style="margin-bottom: 20px;">
    <strong>GET /api/cities Response</strong><br/>
    <img src="" alt="GET Cities Screenshot" style="max-width: 100%; border-radius: 8px; margin-top: 10px;" />
  </div>

  <div style="margin-bottom: 20px;">
    <strong>Nested Attractions Endpoint</strong><br/>
    <img src="" alt="Nested Attractions Screenshot" style="max-width: 100%; border-radius: 8px; margin-top: 10px;" />
  </div>

  <div style="margin-bottom: 20px;">
    <strong>DTOs Overview</strong><br/>
    <img src="" alt="DTOs Screenshot" style="max-width: 100%; border-radius: 8px; margin-top: 10px;" />
  </div>

  <br/>

  <h2 style="color: #333;">📞 Contact</h2>
  <p style="line-height: 1.6; color: #444;">
    If you're a recruiter, engineer, or company looking for a backend developer focused on ASP.NET Core and clean API architecture, feel free to connect with me.
  </p>
  <p>
    <a href="https://www.linkedin.com" target="_blank">📌 Connect on LinkedIn</a>
  </p>

</div>
