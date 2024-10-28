- # Sleeping Condition
  query-table:: true
    |Wake Time|Bed Time|
    |{{query (and [[Wake Time]] (between -7d today))}}|{{query (and [[Bed Time]] (between -7d today))}}|