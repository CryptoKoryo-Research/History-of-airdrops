# History of airdrops

A list of all airdrops that have happened in the past. Here is the corresponding  [Dune dashboard](https://dune.com/cryptokoryo/history-of-airdrops).

>*This repo was created [using this template](https://github.com/duneanalytics/DuneQueryRepo), made to [manage your Dune queries](https://dune.mintlify.app/api-reference/crud/endpoint/create) and any [CSVs as Dune tables](https://dune.mintlify.app/api-reference/upload/endpoint/upload).*

### For Contributors

To add or modify an airdrop, go to the `/uploads` folder and add a row onto an existing CSV sheet or create a new one. It will then get uploaded into Dune as a table. There is currently one CSV called `past_airdrops.csv` that can be queried on Dune as `dune.cryptokoryo_research.dataset_past_airdrops`. The schema we're using for grants right now is below:

| Column Name | Type | Description |
| ----------- | ---- | ----------- |
| `project` | varchar | Name of the project |
| `ticker` | varchar | The symbol/ticker corresponding to the project |
| `category` | timestamp | Category or sector |
| `blockchain` | varbinary | The blockchain to which the project belongs |
| `tier` | double | Airdrop Tier as perceived by the community |
| `date` | varchar | Date at which the airdrop happened |
| `total_amount_airdroped` | int | Total amount ($) airdropped |
| `total_receipeints` | varchar | Total number of airdrop recipients |
| `average_airdropped_per_wallet_dollar` | varchar | Average amount ($) airdropped per walelt |
| `min_allocation` | varchar | Minimum allocation on the airdrop |
| `max_allocation` | varchar | Maximum allocation on the airdrop |

If you want to contribute, either start an issue or go directly into making a PR (using the same labels as above). Once the PR is merged, the queries will get updated in the frontend.

### Query Management Scripts

You'll need python and pip installed to run the script commands. If you don't have a package manager set up, then use either [conda](https://www.anaconda.com/download) or [poetry](https://python-poetry.org/) . Then install the required packages:

```
pip install -r requirements.txt
```





