#Parole Hearing Data

The Parole Hearing Data Project is a repository of New York State parole hearing data based on:

 1. Records scraped from the New York State Parole Board’s website
 2. Parole hearing transcripts crowdsourced with help from attorneys, advocates and prisoners/the formerly incarcerated.

So far, we have gathered 30,000+ records and formatted them for analysis.
Data from a sample run is included in `data.csv`. This project is in development.

We are building this dataset because in New York over 10,000 parole eligible prisoners are denied release every year, and while the consequences of these decisions are costly (at $60,000 annually to incarcerate one individual, and more to incarcerate older individuals with illnesses), the process of how these determinations are made is unclear.

A former parole commissioner stated recently that “[t]he Parole Board process is broken, terribly broken." By gathering substantial data about these determinations, we hope to enable data-driven research that will help identify existing problems and position decision makers well to solve them.

### Setup and run

**Install app requirements**

```bash
$ pip install -r requirements.txt
```

**Running the scraper**

To run the scraper, execute the following python in the base directory of this
repo.

```bash
python scrape.py data.csv > output.csv 2>log.txt &
```

The results of the scraper will be in `output.csv`. Scraper logs will be in
`log.txt`.  The scraper will run in the background, and use the existing
`data.csv` as a source of historical data.

## Team

The Parole Hearing Data Project was created by Nikki Zeichner, a New York City-based criminal defense attorney developing multimedia public projects that explore the U.S. criminal justice system.  Her interest in examining the NYS parole board's release practices grew out of her experience representing a prisoner who had been denied release 9 times before their work together.  More of her storytelling projects can be found at the Museum of the American Prison's website.

Scrapers by Rebecca Ackerman (based on earlier code by R. Luke DuBois and Annie Waldman).

## Errors / Bugs

If something is not behaving intuitively, it is a bug, and should be reported.
Report it here: https://github.com/rcackerman/parole-hearing-data/issues

## Note on Patches/Pull Requests

* Fork the project.
* Make your feature addition or bug fix.
* Send a pull request. Bonus points for topic branches.
