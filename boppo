<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Search Browser</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    #search-container {
      margin-top: 20px;
      text-align: center;
    }

    #results-container {
      margin-top: 20px;
      text-align: left;
    }
  </style>
</head>
<body>

<div id="search-container">
  <h2>Search Browser</h2>
  <input type="text" id="search-input" placeholder="Type your search term">
  <button onclick="search()">Search</button>
</div>

<div id="results-container"></div>

<script>
  const searchResults = [
    { title: 'Result 1', url: 'https://example.com/result1' },
    { title: 'Result 2', url: 'https://example.com/result2' },
    { title: 'Result 3', url: 'https://example.com/result3' },
    // Add more search results as needed
  ];

  function search() {
    const searchTerm = document.getElementById('search-input').value.toLowerCase();
    const resultsContainer = document.getElementById('results-container');
    resultsContainer.innerHTML = ''; // Clear previous results

    const matchingResults = searchResults.filter(result =>
      result.title.toLowerCase().includes(searchTerm)
    );

    if (matchingResults.length === 0) {
      resultsContainer.innerHTML = '<p>No results found.</p>';
    } else {
      matchingResults.forEach(result => {
        const resultElement = document.createElement('div');
        resultElement.innerHTML = `<a href="${result.url}" target="_blank">${result.title}</a>`;
        resultsContainer.appendChild(resultElement);
      });
    }
  }
</script>

</body>
</html>
