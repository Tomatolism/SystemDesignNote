# SystemDesignNote


### Vertical and Horizontal Scaling
Vertical是增大單一Data Base的大小。
Horizontal是，增加多個Database

### Failover server
#### Cold Standby
  定期備份到另外Database，
  優點：便宜、簡單
  缺點：會損失還沒備份到的資料
  
#### Warm Standby
  即時Replication新的資料到備用Database，
  
#### Hot Standby
  直接寫入多個Database
  
#### Sharding Databases

Hotspots：不同資料會有不同的流量，需要監控和調控資料的放置方式。

Normalization Data: 比較少的儲存空間、只要update一個地方的資料。但需要更多query
Denormalization Data: 比較多的儲存空間、Update很困難。但找所要資訊很方便
