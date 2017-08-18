# Using Custom MVC Routes
#### Define custom MVC routes with Route attribute.

In this project I show how to use the Route attribute to change the url associated with a view. 

See the action method `AnyNameHere` in the [HomeController](https://github.com/carlosbocanegra/UsingCustomMVCRoutes/blob/master/Controllers/HomeController.cs)

```csharp
[Route("/MyCustomRoute")]
[Route("/MyCustomRoute/{message}")]
public IActionResult AnyNameHere(string message)
{
    ViewData["Message"] = $"Message: {message}";

    return View("About");
}
```
