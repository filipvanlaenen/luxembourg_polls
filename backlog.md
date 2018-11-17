# Technical Backlog

+ Produce .poll files from a PSV file for each country
+ EP projection:
  - EP Fraction pages
  - Correct the titles for the graphs
  - translate_ep_dichotomies_probabilities_files.rb
  - extract dichotomies confidence intervals (if needed)
+ Rename “Coalitions” into “EP Fractions” and use their proper names for EP
  sites
+ produce_coalitions_*_svg.rb:
  - Produce hatching for all parties, even if they aren't present in the poll
+ produce_*_svg.rb:
  - Add a proper legend for the bars
  - Add local threshold grid line for last results sticking out in the voting
    intentions graph
  - Add local majority grid line for last results sticking out in the seats
    graph
  - Add local majority grid line for last results sticking out in the voting
    intentions graph
  - Darken colors to at least a minimum level
  - Change sorting such that it's according to media first, then upper bound of
    the confidence interval, then the lower bound of the confidence interval,
    and then alphabetically by name, and extend grid lines accordingly
    - Consider to adjust label positions to avoid grid lines
    - Maybe not so relevant any more
+ RSS feed:
  - Sort parties and coalitions according to size (according to graph)
  - Add feed items for coalitions
  - Try to add graphs to Atom feed
+ merge_sapor_results.bsh
  - Merge the state summary files
  - Verify correct convolution of the dichotomies probabilities files
+ Eliminate the need for MajorGridLines and MinorGridLines in country.properties
+ produce_seats_pmf_svgs.bsh:
  - Extend to coalition seats and include in the appropriate pages
  - Extend to voting intentions and include in the appropriate pages
  - Hide grid lines behind the legend
  - Handle long party names in the title (labels for the Y axis may help)
+ produce_trend_svg.rb
  - 95% confidence intervals for every poll, 20%–60%(?) transparent
  - Median in background color, 20%(?) transparent
  - Moving average 95% confidence interval, 50%(?) transparent
  - Moving median, solid line
+ produce_seats_trend_svg.rb
  - 95% confidence intervals for every poll, 20%–60%(?) transparent
  - Median in background color, 20%(?) transparent
  - Moving average 95% confidence interval, 50%(?) transparent
  - Moving median, solid line
+ produce_poll_page.rb:
  - For merged files, display which areas are missing? Or how many?
+ produce_party_page.rb:
  - Add links to these pages from the index, the average and the poll files
  - Add a column with the probability to reach the threshold to the table with
    the confidence intervals for the voting intentions
  - Link to the party page everywhere the party is mentioned
+ Addition to average.md:
  - Better subtitle for the SVGs and PNGs
  - Average only over polls with all areas merged in?
  - Add the probability to reach threshold(s) to the voting intentions table
  - Add the probability to get a majority to the voting intentions and seats
    tables
  - Technical information
    * Field work periods
    * Polling firms included
    * Number of polls included (and pending)
    * Total sample size
    * Largest error estimate
    * Lowest number of simulations
+ Alternative graph:
  - Show differences since last election, with the party gaining the most at the
    top and going to the right, and the party loosing the most at the bottom and
    going to the left
  - Can be done both for voting intentions, seats and coalition seats
  - To be added to every page where the plain graph is shown
+ Handle referendums
  - Change to sapor: produce state_summaries for referendums
  - Remove the seats and coalitions parts of the pages and don't produce the
    graphs
  - Add rankings
+ produce_(average_)coalitions_seats_svg.rb:
  - Switch the order of the masking and the gradient such that the gradient is
    applied to the entire mask as a whole, not to each component individually,
    to remove the color artifacts
+ A page for each polling firm containing all polls for that polling firm
  - Link to the polling firm page everywhere a polling firm is mentioned
  - Add a global page with a list of all polling firms
+ A page for each commissioner containing all polls for that commissioner
  - When a poll has been ordered by more than one commissioner, concatenate
    using '|'
  - Link to the commissioner page everywhere a commissioner is mentioned
  - Add a global page with a list of all commissioners
+ A page for each coalition, similar to the one for parties
+ Global satistics page:
  - Number of polls
  - Total number of simulations
  - Total number of respondents
+ Remove small parties from the all polls table overview
+ Remove absent parties from the average page
+ Make a script to kill the current sapor process such that autorun can continue
  with the next sapor job
+ Make a script to stop autorun and all subprocesses
+ Make it a configurable setting for a country whether the coalition seats
  diagrams should use the parties' full names or abbreviations

# New Countries and Regions

+ Resources for the EU polls website
+ Create Twitter account for eu_polls and add a button for it and to resources
+ Update Norway to the 2017 election (including a new coalition)
+ Update the United Kingdom to the 2017 election
+ Document the results in es-ct-20171221-benchmarking and add them to the methodology
+ Update Catalonia to the 2017 election
+ Italy (4 March 2018)
+ Belgian municipal elections (14 October 2018)
+ Sweden (9 September 2018)
+ Add Brussels
+ Add the French Community in Belgium (convolution of Brussels and Wallonia)
+ Find out about the distribution of seats in Hainaut for the Walloon Parliament
+ Finland (Spring 2019?)
+ Denmark (June 2019?)
+ European Parliament (June 2019)
+ Greece (September 2019?)
+ Poland (October 2019?)
+ Netherlands (spring 2021)?
+ Germany (autumn 2021)?
+ Austria (autumn 2021)?
+ France (spring 2022)?
+ Scotland
+ Bulgaria
+ Catalan referendum
+ Croatia
+ Cyprus
+ Czech Republic
+ Estonia
+ Ireland
+ Latvia
+ Lithuania
+ Luxemburg
+ Malta
+ Portugal
+ Romania
+ Slovakia
+ Slovenia
+ Spain
+ Switserland
+ Australia
+ Canada
+ Israel
+ Japan
+ New Zealand
+ US

# Uniform Twitter handles

## Current

+ Belgium: belpolls
+ Catalonia: catpolls
+ Great Brittain: gbrpolls
+ Greece: grpolls → grcpolls
+ Hungary: hunpolls
+ Iceland: islpolls
+ Norway: norpolls
+ Scotland: scotpolls → sctpolls
+ Slovenia: svnpolls
+ Sweden: swepolls

## Future

+ Bulgaria: bgrpolls
+ Croatia: hrvpolls
+ Cyprus: cyppolls
+ Czech Republic: czepolls
+ Denmark: dnkpolls
+ Estonia: estpolls
+ Finland: finpolls
+ France: frapolls
+ Germany: deupolls
+ Ireland: irlpolls
+ Italy: itapolls
+ Latvia: lvapolls
+ Lithuania: ltupolls
+ Luxemburg: luxpolls
+ Malta: mltpolls
+ Netherlands: nldpolls
+ Poland: polpolls
+ Portugal: prtpolls
+ Romania: roupolls
+ Slovakia: svkpolls
+ Spain: esppolls
