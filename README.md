# WebScraping-Challenge

## Table of Content
- part_1_mars_news-fin.ipynb
- part_2_mars_weather-fin.ipynb
- output.csv

## References of code sourced from
- Monash Lesson Plans - Data Collection
- Stack Overflow
- AskBCs Richie, assisted in cleaning up following code:
    # code
    # Extract all rows of data
      tr_rows = soup.find_all('tr', class_="data-row")
      tr_rows
    # code
    # Loop through the scraped data to create a list of rows
      for row in tr_rows:
        td = row.find_all('td')
        row = [col.text for col in td]
        mars_row.append(row)

    # code
    # How many terrestrial (earth) days are there in a Martian year?
    mars_df.min_temp.plot()
    plt.xlabel('Number of terrestrial days')
    plt.ylabel('Minimum temperature')
    plt.show()
    
