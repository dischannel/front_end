# front_end
Performance 时间定义

readyStart = timing.fetchStart - timing.navigationStart; // 准备新页面时间耗时
redirectTime = timing.redirectEnd - timing.redirectStart; // 重定向耗时
appcacheTime = timing.domainLookupStart - timing.fetchStart; // Appcache 耗时
unloadEventTime = timing.unloadEventEnd - timing.unloadEventStart; // unload 前文档耗时
lookupDomainTime = timing.domainLookupEnd - timing.domainLookupStart; // DNS 查询耗时
connectTime = timing.connectEnd - timing.connectStart; // TCP连接耗时
requestTime = timing.responseEnd - timing.requestStart; // request请求耗时
initDomTreeTime = timing.domInteractive - timing.responseEnd; // 请求完毕至DOM加载:
domReadyTime = timing.domComplete - timing.domInteractive; // 解释dom树耗时:
loadTime = timing.loadEventEnd - timing.navigationStart // 从开始至load总耗时:
