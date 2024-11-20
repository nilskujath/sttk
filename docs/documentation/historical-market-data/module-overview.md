# Module Overview


The `HistoricalMarketDataCollector` module is designed to fetch historical market data from 
various sources, process it into pandas DataFrames, and then store the data in user-specified formats. 
It ensures flexible configuration of the historical market data retrieval process 
through a **dictionary-based initialization**, as per the example below:

```python
config = {
    "source": "yfinance",
    "storage_option": "csv",
    "storage_dir": "../sttk-data/csv/",
    "list_of_tickers": ["AAPL", "MSFT"],
    "start_date": "2023-01-01",
    "end_date": "2023-03-01",
    "interval": {"day": 1},
}

collector = HistoricalMarketDataCollector(config)
collector.get_data()
```

The following table summarizes the possible parameters that can be ingested at the
instantiation of the `HistoricalDataCollector` class:

| Parameter             | Type                | Description                                                                                                                                                                    |
|-----------------------|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `source`              | `str`               | Data source. [:octicons-arrow-right-24: See Supported Data Sources](supported-data-sources.md)                                                                                 |
| `storage_option`      | `str`               | Storage format. [:octicons-arrow-right-24: See Supported Storage Options](supported-storage-options.md)                                                                        |
| `storage_dir`         | `str`               | Directory path where data will be saved.<br> Example: `"../sttk-data/csv"`                                                                                                     |
| `list_of_tickers`     | `List[str]`         | List of ticker symbols for which data should be collected.<br> Example: `["AAPL", "MSFT"]`                                                                                     |
| `start_date`          | `str` or `datetime` | Starting date for data retrieval.<br> Example: `2023-01-01` or `datetime.datetime(2023, 1, 1)`                                                                                 | 
| `end_date`            | `str` or `datetime` | Optional (!) ending date.<br> Note: *Defaults to the current date if not provided.*                                                                                            |
| `interval`            | `Dict[str, int]`    | Dictionary specifying the interval type and duration.<br> [:octicons-arrow-right-24: See Supported Interval Types](../ontology/non-event-types.md) <br> Example: `{"hour": 1}` |
