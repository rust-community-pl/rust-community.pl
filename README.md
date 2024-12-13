# Rust Poland community index
This repository contains the source data for the https://rust-community.pl  website, which serves as an index of communities, events and other things related to the Rust language in Poland. 

## Contributing
You can send a pull request to add new content. Data for the index is automatically generated from the following files:

- `data/communities.yaml` - online communities and discussion forums
- `data/events.yaml` - events related to Rust in Poland
- `data/education.yaml` - Rust courses taught at universities
- `data/recordings.yaml` - recordings of Rust content (e.g. from meetups and conferences)
- `data/trainings.yaml` - Rust training offerings
- `data/companies.yaml` - companies using Rust

Note that all added content should be relevant to Rust usage in Poland, as this index is focused on the local Rust community.

## Build instructions
1) Install [Zola](https://www.getzola.org/documentation/getting-started/installation/)
2) (Optional) Build RSS feed
    ```bash
    $ cd rss
    $ cargo run -- --data-path ../data ../static/feed.xml 
    ```
3) Run `zola serve` or `zola build`

