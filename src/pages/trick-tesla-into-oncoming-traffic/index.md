---
title: Tesla Autopilot Tricked Into Steering Into Oncoming Traffic
date: '2019-04-02'
spoiler: Researchers have devised a simple attack that might cause a Tesla to automatically steer into oncoming traffic under certain conditions. The proof-of-concept exploit works not by hacking into the car’s onboard computing system. Instead, it works by using small, inconspicuous stickers that trick the Enhanced Autopilot of a Model S 75 into detecting and then following a change in the current lane. Researchers from Tencent’s Keen Security Lab recently reverse-engineered several of Tesla’s automated processes to see how they reacted when environmental variables changed.
---
![UConn](./Tesla.jpg)

Researchers have devised a simple attack that might cause a Tesla to automatically steer into oncoming traffic under certain conditions as reported on [BlastBoard](https://www.blastboard.com/t/researchers-trick-tesla-autopilot-into-steering-into-oncoming-traffic/35). The proof-of-concept exploit works not by hacking into the car’s onboard computing system. Instead, it works by using small, inconspicuous stickers that trick the Enhanced Autopilot of a Model S 75 into detecting and then following a change in the current lane. Researchers from Tencent’s Keen Security Lab recently reverse-engineered several of Tesla’s automated processes to see how they reacted when environmental variables changed.

The researchers noted that Autopilot uses a variety of measures to prevent incorrect detections. The measures include the position of road shoulders, lane histories, and the size and distance of various object. [A section of the researchers’ 37-page report] showed how researchers could tamper with a Tesla’s autowiper system to activate wipers on when rain wasn’t falling. Unlike traditional autowiper systems – which use optical sensors to detect moisture – Tesla’s system uses a suite of cameras that feeds data into an artificial intelligence network to determine when wipers should be turned on. 

The researchers found that – in much the way it’s easy for small changes in an image to throw off artificial intelligence-based image recognition (for instance, changes that cause an AI system to mistake a panda for a gibbon) – it wasn’t hard to trick Tesla’s autowiper feature into thinking rain was falling even when it was not. So far, the researchers have only been able to fool autowiper when they feed images directly into the system. Eventually, they said, it may be possible for attackers to display an “adversarial image” that’s displayed on road signs or other cars that do the same thing. In a statement, Tesla officials said that the vulnerabilities addressed in the report have been fixed via security update in 2017, “followed by another comprehensive security update in 2018, both of which we released before this group reported this research to us.” 

<!-- TradingView Widget BEGIN -->
<div class="tradingview-widget-container">
  <div id="tradingview_088e4"></div>
  <div class="tradingview-widget-copyright"><a href="https://www.tradingview.com/symbols/NASDAQ-AAPL/" rel="noopener" target="_blank"><span class="blue-text">AAPL Chart</span></a> by TradingView</div>
  <script type="text/javascript" src="https://s3.tradingview.com/tv.js"></script>
  <script type="text/javascript">
  new TradingView.widget(
  {
  "width": 980,
  "height": 610,
  "symbol": "NASDAQ:AAPL",
  "interval": "D",
  "timezone": "Etc/UTC",
  "theme": "Light",
  "style": "1",
  "locale": "en",
  "toolbar_bg": "#f1f3f6",
  "enable_publishing": true,
  "allow_symbol_change": true,
  "details": true,
  "news": [
    "headlines"
  ],
  "container_id": "tradingview_088e4"
}
  );
  </script>
</div>
<!-- TradingView Widget END -->