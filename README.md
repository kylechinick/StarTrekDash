# _StarTrek Dash_

#### By _Chief Science Officer Ashe Urban Chief Medical Officer Caroline Cerussi Captian of Engineering Claire Thorington Councelor Kyle Chinick Ensign Justin Peters Chief Engineer Liam Campbell_

#### _A C# based Star Trek Dashboard_

## Table of Contents

[Technologies Used](#technologies-used)  
[Description](#description)  
[Setup/Installation Requirements](#setup-and-installation-requirements)  
[Known Bugs](#known-bugs)  
[License](#License)

## Technologies Used

- _C#_
- _.NET_
- _RestSharp_
- _SQL Workbench_
- _Entity Framework_
- _MVC_

## APIs Used

### WEATHERBIT

- _API Source:_ https://rapidapi.com/weatherbit/api/weather/
- _API Registration:_ https://rapidapi.com/auth/sign-up?referral=/weatherbit/api/weather/
- _API Endpoint Documentation:_ https://www.weatherbit.io/api/weather-current

### NY TIMES

- _API Source:_ https://developer.nytimes.com/apis
- _API Registration:_ https://developer.nytimes.com/accounts/create
- _API Endpoint Documentation:_ https://developer.nytimes.com/docs/top-stories-product/1/overview

## Visual Sources

- _LCARS Theme:_ https://www.thelcars.com by Jim Robertus
- _Enterprise Line Illustration:_ https://favpng.com/png_view/star-enterprise-starship-enterprise-star-trek-uss-enterprise-ncc-1701-png/J6pEmXpv by User Lulzboatz, https://favpng.com/png_user/Lulzboatz
- _Enterprise Diagram & Key:_ https://wall.alphacoders.com/big.php?i=321822

---

## Description

_This is a Star Trek Themed Dashboard. Provides weather data for San Francisco, CA grabs science news from the NYT Api and displays them all in one place in a slick StarTrek Themed space._

---

## Setup and Installation Requirements

<details>
<summary><strong>Initial Setup</strong></summary>
<ol>
<li>Clone this repository to your local machine by running the following command in your preferred terminal application:

```Shell
git clone https://github.com/AsheUrban/StarTrekDash.git
```

_Note:_ for Primary Fork/Team Repo visit, https://github.com/carolinecerussi/StarTrekDash.git

<li>Navigate to the root directory – StarTrekDash.
<br>
</details>

<details>
<summary><strong>SQL Workbench Configuration</strong></summary>
<ol>
<li>Create an appsetting.json file in the root directory of the project and add to your .gitignore file*  
   <pre>StarTrekDash
   └── StarTrekDash
    └── appsetting.json</pre>
<li> Insert the following code** : <br>

<pre>{
   "Logging": {
    "LogLevel": {
      "Default": "Warning",
      "System": "Information",
      "Microsoft": "Information"
    }
  },
  "AllowedHosts": "*"
</pre>

</details>

<details>
<summary><strong>To Run</strong></summary>
Navigate to:  
   <pre>StarTrek_Dash
   └── <strong>StarTrekDash</strong></pre>

Run `$ dotnet restore`<br>
Run `$ dotnet build` <br>
Run `$ dotnet run` <br>

</details>

<br>

This program was built using _`Microsoft .NET SDK 5.0.401`_, and may not be compatible with other versions. Your milage may vary.

## Known Bugs & Stretch Goals

- _Once weather API runs out of calls, application breaks. Possible fix is hosting seperate APIhelpers for each API. To continue running application, visit API documenation and reregister with a new email address._

- _LaunchAPI was built, but not successfully integrated._
  https://github.com/JPeters25/Launch_Api.git<br>
- _Star Trek Audio Clips not integrated._ <br>
  https://trekcore.com/audio/<br>

## License

MIT

[Copyright](/LICENSE) (c) _08-21-2022_ _Ashe Urban Caroline Cerussi Claire Thorington Kyle Chinnick Justin Peters Liam Campbell_
