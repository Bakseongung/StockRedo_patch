### StockRedo v0.0.1.md
```
주식 시뮬레이터(계속 패치중)
1 --- 가상자산, 실제 주식시장 반영
2 --- 국내 모든 주식 가능(ETF 아직 제외)
3 --- 실시간 수집 : 평일 08:50 ~ 15:40, 평균 13초마다 Redis를 갱신 (Systemd 서비스)
4 --- 영구 적재 : 1분마다 MySQL에 스냅샷 저장 (Crontab + archiver.py)
5 --- 자동 청소 : 7일 지난 데이터는 MySQL이 스스로 삭제 (MySQL Event Scheduler)
```
