<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
      integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T"
      crossorigin="anonymous"
    />
    <script src="https://unpkg.com/axios/dist/axios.min.js"></script>
    <link rel="stylesheet" href="src/styles.css" />
    <title>Weather App</title>
  </head>

  <body>
    <div class="container">
      <div class="weather-app">
        <form class="search-form" id="search-form">
          <div class="row">
            <div class="col-9">
              <input
                type="search"
                placeholder="Type a city.."
                autofocus="on"
                autocomplete="off"
                id="city-input"
                class="form-control shadow-sm"
              />
            </div>
            <div class="col-3">
              <button
                class="btn btn-success w-100"
                id="current-location-button"
              >
                Current
              </button>
            </div>
          </div>
        </form>
        <h1 id="city">Sydney NSW, Australia</h1>
        <ul>
          <li id="date"></li>
          <li>Partly Cloudy</li>
        </ul>
        <div class="row">
          <div class="col-6">
            <div class="clearfix">
              <img
                src="https://ssl.gstatic.com/onebox/weather/64/partly_cloudy.png"
                alt="Cloudy icon"
                class="weather-icon float-left"
              />
              <div class="float-left">
                <span class="temperature" id="temperature">19</span
                ><span class="units">
                  <a href="#" id="celsius-link">°C</a> |
                  <a href="#" id="fahrenheit-link">°F</a>
                </span>
              </div>
            </div>
          </div>
          <div class="col-6">
            <ul>
              <li>Precipitation: 0%</li>
              <li>Humidity: 77%</li>
              <li>Wind: 8 km/h</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <script>
      function formatDate(date) {
        let hours = date.getHours();
        if (hours < 10) {
          hours = `0${hours}`;
        }
        let minutes = date.getMinutes();
        if (minutes < 10) {
          minutes = `0${minutes}`;
        }

        let dayIndex = date.getDay();
        let days = [
          "Sunday",
          "Monday",
          "Tuesday",
          "Wednesday",
          "Thursday",
          "Friday",
          "Saturday",
        ];

        let day = days[dayIndex];

        return `${day} ${hours}:${minutes}`;
      }

      function displayWeatherCondition(response) {
        document.querySelector("#city").innerHTML = response.data.name;
        document.querySelector("#temperature").innerHTML = Math.round(
          response.data.main.temp
        );

        document.querySelector("#humidity").innerHTML =
          response.data.main.humidity;
        document.querySelector("#wind").innerHTML = Math.round(
          response.data.wind.speed
        );
        document.querySelector("#description").innerHTML =
          response.data.weather[0].main;
      }

      function searchCity(city) {
        let apiKey = "5f472b7acba333cd8a035ea85a0d4d4c";
        let apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}&units=metric`;
        axios.get(apiUrl).then(displayWeatherCondition);
      }

      function handleSubmit(event) {
        event.preventDefault();
        let city = document.querySelector("#city-input").value;
        searchCity(city);
      }

      function searchLocation(position) {
        let apiKey = "5f472b7acba333cd8a035ea85a0d4d4c";
        let apiUrl = `https://api.openweathermap.org/data/2.5/weather?lat=${position.coords.latitude}&lon=${position.coords.longitude}&appid=${apiKey}&units=metric`;

        axios.get(apiUrl).then(displayWeatherCondition);
      }

      function getCurrentLocation(event) {
        event.preventDefault();
        navigator.geolocation.getCurrentPosition(searchLocation);
      }

      function convertToFahrenheit(event) {
        event.preventDefault();
        let temperatureElement = document.querySelector("#temperature");
        temperatureElement.innerHTML = 66;
      }

      function convertToCelsius(event) {
        event.preventDefault();
        let temperatureElement = document.querySelector("#temperature");
        temperatureElement.innerHTML = 19;
      }

      let dateElement = document.querySelector("#date");
      let currentTime = new Date();
      dateElement.innerHTML = formatDate(currentTime);

      let searchForm = document.querySelector("#search-form");
      searchForm.addEventListener("submit", handleSubmit);

      let currentLocationButton = document.querySelector(
        "#current-location-button"
      );
      currentLocationButton.addEventListener("click", getCurrentLocation);

      searchCity("New York");
    </script>
  </body>
</html>
