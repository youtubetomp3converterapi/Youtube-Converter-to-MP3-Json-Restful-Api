# Free Unlimited Youtube Json Rest Api
For each use case, the tool displays the parameters used in the API request. You can modify the parameter values, in which case the tool updates the code snippets to reflect the parameter values that you provided. The tool also displays the API response to each request. If you have modified the request parameters, the API response is based on your provided parameter values.
<h4 class="panel-title panel-heading">Send an HTTP request to:</h4>
<pre class="prettyprint lang-html">https://video.download-lagu-mp3.com/@api/json/<b><span class="nocode" style="color:#65b042">{format}</span></b>/<b><span class="nocode" style="color:#65b042">{YouTube-Video-ID}</span></b></pre>
<h4 class="panel-title panel-heading">Where <code><b>{format}</b></code> is one of the following:</h4>
<div class="panel-title panel-heading">
<ul style="margin-bottom:0">
<li>"<b>mp3</b>" : for MP3 results</li>
<li>"<b>videos</b>" : for Video w/Audio results</li>
<li>"<b>videostreams</b>" : for Video-Only results</li>
<li>"<b>audiostreams</b>" : for Audio-Only results</li>
</ul>
</div>
<h4 class="panel-title panel-heading">And <code><b>{YouTube-Video-ID}</b></code> is any valid YouTube video ID.</h4>
<h4 class="panel-title panel-heading">The API request and corresponding JSON response should look like one of the following, e.g.:</h4>
<div>

<div class="panel-heading">
<ul class="nav nav-tabs" role="tablist">
<li role="presentation" class="active"><a href="#mp3-json-api" aria-controls="home" role="tab" data-toggle="tab">MP3</a></li>
<li role="presentation"><a href="#videos-json-api" aria-controls="profile" role="tab" data-toggle="tab">Video w/Audio</a></li>
<li role="presentation"><a href="#videostreams-json-api" aria-controls="messages" role="tab" data-toggle="tab">Video-Only</a></li>
<li role="presentation"><a href="#audiostreams-json-api" aria-controls="settings" role="tab" data-toggle="tab">Audio-Only</a></li>
</ul>
</div>

<div class="tab-content">
<div role="tabpanel" class="tab-pane fade in active" id="mp3-json-api">
<pre class="prettyprint lang-html">GET https://video.download-lagu-mp3.com/@api/json/mp3/CevxZvSJLk8 HTTP/1.1</pre>
<h4 class="panel-title panel-heading">Generates this:</h4>
<pre class="prettyprint lang-php">{
	"vidID": "CevxZvSJLk8",
	"vidTitle": "Katy Perry - Roar (Official)",
	"vidInfo": {
		"0": {
			"dloadUrl": "//video.download-lagu-mp3.com/@download/320-58e7c0e582ce2-10800000/mp3/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp3",
			"bitrate": 320,
			"mp3size": "10.3 MB"
		},
		"1": {
			"dloadUrl": "//video.download-lagu-mp3.com/@download/256-58e7c0e582ce2-8640000/mp3/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp3",
			"bitrate": 256,
			"mp3size": "8.24 MB"
		},
		"2": {
			"dloadUrl": "//video.download-lagu-mp3.com/@download/192-58e7c0e582ce2-6480000/mp3/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp3",
			"bitrate": 192,
			"mp3size": "6.18 MB"
		},
		"3": {
			"dloadUrl": "//video.download-lagu-mp3.com/@download/128-58e7c0e582ce2-4320000/mp3/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp3",
			"bitrate": 128,
			"mp3size": "4.12 MB"
		},
		"4": {
			"dloadUrl": "//video.download-lagu-mp3.com/@download/64-58e7c0e582ce2-2160000/mp3/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp3",
			"bitrate": 64,
			"mp3size": "2.06 MB"
		}
	}
}</pre>
</div>
<div role="tabpanel" class="tab-pane fade" id="videos-json-api">
<pre class="prettyprint lang-html">GET https://video.download-lagu-mp3.com/@api/json/videos/CevxZvSJLk8 HTTP/1.1</pre>
<h4 class="panel-title panel-heading">Generates this:</h4>
<pre class="prettyprint lang-php">{
	"vidID": "CevxZvSJLk8",
	"vidTitle": "Katy Perry - Roar (Official)",
	"vidInfo": {
		"0": {
			"rSize": "67.79 MB",
			"quality": "720",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?ipbits=0&mm=31&mn=sn-5uh5o-f5f6&itag=22&mt=1492837642&dur=269.165&id=o-AB1T_kZWIIiA_ihhSlAK4RXegp3Z9A18zn39hF0Aa51G&initcwndbps=197500&pl=21&source=youtube&mv=m&ip=137.74.1.176&mime=video%2Fmp4&ms=au&ratebypass=yes&requiressl=yes&sparams=dur%2Cei%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpl%2Cratebypass%2Crequiressl%2Csource%2Cupn%2Cexpire&key=yt6&lmt=1478841669593636&upn=Wp652d9rFKo&ei=OuX6WLqMDJaLNK-MmLAE&expire=1492859290&signature=A8B328D48101C553D0659D2D9D1F1B2F249D2035.792897E2CF6BFEFC97C81A90EA9CBF9B76FD0283&type=video%252Fmp4%253B%2Bcodecs%253D%2522avc1.64001F%252C%2Bmp4a.40.2%2522&quality=hd720&title=Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/22-58fae53acfc14-mp4-71087585/videos/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "",
			"bitrate": "",
			"codec": "",
			"itag": "22",
			"vidid": "CevxZvSJLk8"
		},
		"1": {
			"rSize": "27.24 MB",
			"quality": "360",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?ipbits=0&mm=31&mn=sn-5uh5o-f5f6&itag=43&mt=1492837642&dur=0.000&id=o-AB1T_kZWIIiA_ihhSlAK4RXegp3Z9A18zn39hF0Aa51G&initcwndbps=197500&pl=21&source=youtube&mv=m&ip=137.74.1.176&mime=video%2Fwebm&ms=au&ratebypass=yes&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpl%2Cratebypass%2Crequiressl%2Csource%2Cupn%2Cexpire&gir=yes&clen=28559516&key=yt6&lmt=1378406587282120&upn=Wp652d9rFKo&ei=OuX6WLqMDJaLNK-MmLAE&expire=1492859290&signature=034E22ACDCD519B206F57F4E83531F20E02B44CE.0F2F6F68AEDA962A6FE339B396CEB1C9AFC76BEB&type=video%252Fwebm%253B%2Bcodecs%253D%2522vp8.0%252C%2Bvorbis%2522&quality=medium&title=Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/43-58fae53acfc14-webm-28559516/videos/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "",
			"bitrate": "",
			"codec": "",
			"itag": "43",
			"vidid": "CevxZvSJLk8"
		},
		"2": {
			"rSize": "23.04 MB",
			"quality": "360",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?ipbits=0&mm=31&mn=sn-5uh5o-f5f6&itag=18&mt=1492837642&dur=269.165&id=o-AB1T_kZWIIiA_ihhSlAK4RXegp3Z9A18zn39hF0Aa51G&initcwndbps=197500&pl=21&source=youtube&mv=m&ip=137.74.1.176&mime=video%2Fmp4&ms=au&ratebypass=yes&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpl%2Cratebypass%2Crequiressl%2Csource%2Cupn%2Cexpire&gir=yes&clen=24160662&key=yt6&lmt=1478829646729343&upn=Wp652d9rFKo&ei=OuX6WLqMDJaLNK-MmLAE&expire=1492859290&signature=270317DE0C7738F41DCCD1C57CB00E4016E72863.9534418D093B61007460C6EE1E3442BF14F923E0&type=video%252Fmp4%253B%2Bcodecs%253D%2522avc1.42001E%252C%2Bmp4a.40.2%2522&quality=medium&title=Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/18-58fae53acfc14-mp4-24160662/videos/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "",
			"bitrate": "",
			"codec": "",
			"itag": "18",
			"vidid": "CevxZvSJLk8"
		},
		"3": {
			"rSize": "7.3 MB",
			"quality": "240",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?ipbits=0&mm=31&mn=sn-5uh5o-f5f6&itag=36&mt=1492837642&dur=269.306&id=o-AB1T_kZWIIiA_ihhSlAK4RXegp3Z9A18zn39hF0Aa51G&initcwndbps=197500&pl=21&source=youtube&mv=m&ip=137.74.1.176&mime=video%2F3gpp&ms=au&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&gir=yes&clen=7651100&key=yt6&lmt=1384321001624346&upn=Wp652d9rFKo&ei=OuX6WLqMDJaLNK-MmLAE&expire=1492859290&signature=35D4FA5FB1407310FFBAD2B025B7A90589C3DDDC.AF6B508B592A2D99C22E09D8AF595D5A6F18DE17&type=video%252F3gpp%253B%2Bcodecs%253D%2522mp4v.20.3%252C%2Bmp4a.40.2%2522&quality=small&ratebypass=yes&title=Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/36-58fae53acfc14-3gp-7651100/videos/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.3gp",
			"ftype": "3gp",
			"framerate": "",
			"bitrate": "",
			"codec": "",
			"itag": "36",
			"vidid": "CevxZvSJLk8"
		},
		"4": {
			"rSize": "2.64 MB",
			"quality": "144",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?ipbits=0&mm=31&mn=sn-5uh5o-f5f6&itag=17&mt=1492837642&dur=269.492&id=o-AB1T_kZWIIiA_ihhSlAK4RXegp3Z9A18zn39hF0Aa51G&initcwndbps=197500&pl=21&source=youtube&mv=m&ip=137.74.1.176&mime=video%2F3gpp&ms=au&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&gir=yes&clen=2769777&key=yt6&lmt=1384320873661266&upn=Wp652d9rFKo&ei=OuX6WLqMDJaLNK-MmLAE&expire=1492859290&signature=6E5A508E54E1CFA5E692F4D38962DF6DAD8AD9D4.7225B93B923384F0F6319249B81E2A9FE68FF8F6&type=video%252F3gpp%253B%2Bcodecs%253D%2522mp4v.20.3%252C%2Bmp4a.40.2%2522&quality=small&ratebypass=yes&title=Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/17-58fae53acfc14-3gp-2769777/videos/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.3gp",
			"ftype": "3gp",
			"framerate": "",
			"bitrate": "",
			"codec": "",
			"itag": "17",
			"vidid": "CevxZvSJLk8"
		}
	}
}</pre>
</div>
<div role="tabpanel" class="tab-pane fade" id="videostreams-json-api">
<pre class="prettyprint lang-html">GET https://video.download-lagu-mp3.com/@api/json/videostreams/CevxZvSJLk8 HTTP/1.1</pre>
<h4 class="panel-title panel-heading">Generates this:</h4>
<pre class="prettyprint lang-php">{
	"vidID": "CevxZvSJLk8",
	"vidTitle": "Katy Perry - Roar (Official)",
	"vidInfo": {
		"0": {
			"rSize": "116.17 MB",
			"quality": "1080",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=1920x1080&initcwndbps=215000&dur=269.102&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=121811386&itag=137&requiressl=yes&ip=193.70.125.81&mime=video%2Fmp4&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1478838201195116&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=1080p&signature=8AF48B22377AF753307928612997EBFC0C08B054.6B9606A89C62EEC56D229FCDD81DC1FDB19F656F&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/137-58fae9948011d-mp4-121811386/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "137",
			"vidid": "CevxZvSJLk8"
		},
		"1": {
			"rSize": "84.36 MB",
			"quality": "1080",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=1920x1080&initcwndbps=215000&dur=269.060&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=88457561&itag=248&requiressl=yes&ip=193.70.125.81&mime=video%2Fwebm&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1449556089462409&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=1080p&signature=1744D650EF084EBB6FCEAD6E0D81B5613EFDFE4B.777290054FE1278E26E74E478A62A5E107683EE6&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/248-58fae9948011d-webm-88457561/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "248",
			"vidid": "CevxZvSJLk8"
		},
		"2": {
			"rSize": "63.73 MB",
			"quality": "720",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=1280x720&initcwndbps=215000&dur=269.102&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=66825779&itag=136&requiressl=yes&ip=193.70.125.81&mime=video%2Fmp4&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1478841623640509&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=720p&signature=09522FA5C11047F974F657618AE8EBB4F6A74357.B23C4D708531BF2EEE743316CF2205CA0C62DD09&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/136-58fae9948011d-mp4-66825779/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "136",
			"vidid": "CevxZvSJLk8"
		},
		"3": {
			"rSize": "47.71 MB",
			"quality": "720",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=1280x720&initcwndbps=215000&dur=269.060&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=50030690&itag=247&requiressl=yes&ip=193.70.125.81&mime=video%2Fwebm&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1449556446128414&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=720p&signature=BA1B00A4CF28F1777A102F00A164D554AE960E7B.26761B8279B43EBD9DFF95E9C44D43956987AA51&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/247-58fae9948011d-webm-50030690/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "247",
			"vidid": "CevxZvSJLk8"
		},
		"4": {
			"rSize": "32.97 MB",
			"quality": "480",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=854x480&initcwndbps=215000&dur=269.102&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=34568157&itag=135&requiressl=yes&ip=193.70.125.81&mime=video%2Fmp4&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1478841623657218&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=480p&signature=1B3533F6C960B14DF1C74E3E94BC34EFBF3B9FA0.04294BAC58A3440A100464FF53B1B5CE9978C724&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/135-58fae9948011d-mp4-34568157/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "135",
			"vidid": "CevxZvSJLk8"
		},
		"5": {
			"rSize": "24.28 MB",
			"quality": "480",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=854x480&initcwndbps=215000&dur=269.060&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=25458088&itag=244&requiressl=yes&ip=193.70.125.81&mime=video%2Fwebm&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1449556444988251&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=480p&signature=21CCCAFF261EFB14C6754AA1DB32D994CFF6BA3B.6427E42361C1678BBE283865E13D37916EC1A6B9&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/244-58fae9948011d-webm-25458088/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "244",
			"vidid": "CevxZvSJLk8"
		},
		"6": {
			"rSize": "17.48 MB",
			"quality": "360",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=640x360&initcwndbps=215000&dur=269.102&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=18325768&itag=134&requiressl=yes&ip=193.70.125.81&mime=video%2Fmp4&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1478841619832595&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=360p&signature=9E0C1DC96E9DC16263F5A6C4F6F3C6BBC11EA27E.153CCC7776ABDDAA73B85C155E86AC399F46AC5C&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/134-58fae9948011d-mp4-18325768/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "134",
			"vidid": "CevxZvSJLk8"
		},
		"7": {
			"rSize": "13.18 MB",
			"quality": "360",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=640x360&initcwndbps=215000&dur=269.060&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=13821316&itag=243&requiressl=yes&ip=193.70.125.81&mime=video%2Fwebm&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1449556444122717&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=360p&signature=407D6EB829F979FD6FE07B6A1B03D256F8FF8722.DB4051B0582C0F75C9E6DC4690B301C1C6464D59&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/243-58fae9948011d-webm-13821316/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "243",
			"vidid": "CevxZvSJLk8"
		},
		"8": {
			"rSize": "7.28 MB",
			"quality": "240",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=426x240&initcwndbps=215000&dur=269.102&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=7637886&itag=133&requiressl=yes&ip=193.70.125.81&mime=video%2Fmp4&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1478841618531765&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=240p&signature=BB53FD73632DA30E807F914F671D546824DDF91E.1172799335FD03BC679608A0C2E068CE3641997E&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/133-58fae9948011d-mp4-7637886/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "133",
			"vidid": "CevxZvSJLk8"
		},
		"9": {
			"rSize": "7.16 MB",
			"quality": "240",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=426x240&initcwndbps=215000&dur=269.060&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=7505220&itag=242&requiressl=yes&ip=193.70.125.81&mime=video%2Fwebm&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1449556444140323&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=240p&signature=E39882E6EDD10AD5E7A76B602F47F2E7ED2E7397.38E334B584817BB3809C984B4D94A51638F75CF6&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/242-58fae9948011d-webm-7505220/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "30",
			"bitrate": "",
			"codec": "",
			"itag": "242",
			"vidid": "CevxZvSJLk8"
		},
		"10": {
			"rSize": "3.28 MB",
			"quality": "144",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=24&size=256x144&initcwndbps=215000&dur=269.102&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=3440468&itag=160&requiressl=yes&ip=193.70.125.81&mime=video%2Fmp4&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1478841619229633&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=144p&signature=4EADC74169CFA8D0EBCBCBD9C2DC5736C1DC0D67.4531249CE707CF142EED7C7BE1E4BD2390601E35&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/160-58fae9948011d-mp4-3440468/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.mp4",
			"ftype": "mp4",
			"framerate": "15",
			"bitrate": "",
			"codec": "",
			"itag": "160",
			"vidid": "CevxZvSJLk8"
		},
		"11": {
			"rSize": "3.18 MB",
			"quality": "144",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?fps=12&size=256x144&initcwndbps=215000&dur=269.018&upn=M8eDc-KBrLU&key=yt6&keepalive=yes&clen=3338486&itag=278&requiressl=yes&ip=193.70.125.81&mime=video%2Fwebm&mn=sn-5uh5o-f5f6&pl=23&source=youtube&mm=31&ms=au&id=o-AD09h7_FeC3HX73KtXA-t8LLln90DWmWeQ5Dcfx9FjOU&mv=m&mt=1492838725&expire=1492860403&gir=yes&lmt=1449556443708071&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2cms%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&ei=k-n6WPDgJo_Cdo_Fm7AO&ipbits=0&pcm2cms=yes&quality_label=144p&signature=3AED4867AFD392B513BC04698AE858DAE9B7F003.4FE03F31B31F237CBE01CC5DCE9A55107B27ED60&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/278-58fae9948011d-webm-3338486/videostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "15",
			"bitrate": "",
			"codec": "",
			"itag": "278",
			"vidid": "CevxZvSJLk8"
		}
	}
}</pre>
</div>
<div role="tabpanel" class="tab-pane fade" id="audiostreams-json-api">
<pre class="prettyprint lang-html">GET https://video.download-lagu-mp3.com/@api/json/audiostreams/CevxZvSJLk8 HTTP/1.1</pre>
<h4 class="panel-title panel-heading">Generates this:</h4>
<pre class="prettyprint lang-php">{
	"vidID": "CevxZvSJLk8",
	"vidTitle": "Katy Perry - Roar (Official)",
	"vidInfo": {
		"0": {
			"rSize": "4.08 MB",
			"quality": "",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?mt=1492841663&mv=m&initcwndbps=183750&ipbits=0&ms=au&mm=31&mn=sn-5uh5o-f5f6&ip=137.74.1.176&key=yt6&keepalive=yes&source=youtube&clen=4275631&pcm2=no&lmt=1478829623441921&gir=yes&upn=3Cks0aHaVpw&pl=21&expire=1492863364&id=o-AGPeW3bkX1nrk-fjCVQFZIVsUdAaHNbcsWsG0M2V8e4u&itag=140&mime=audio%2Fmp4&dur=269.165&ei=JPX6WJ3rJJegd7zqodgJ&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&signature=D602D3604E3B7911EDE4AF1E7D9EDD61F8524DF6.0CFF23E3A835992CA48134DB1CE2A20297591671&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/140-58faf5254fc43-m4a-4275631/audiostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.m4a",
			"ftype": "m4a",
			"framerate": "",
			"bitrate": "128",
			"codec": "AAC",
			"itag": "140",
			"vidid": "CevxZvSJLk8"
		},
		"1": {
			"rSize": "3.83 MB",
			"quality": "",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?mt=1492841663&mv=m&initcwndbps=183750&ipbits=0&ms=au&mm=31&mn=sn-5uh5o-f5f6&ip=137.74.1.176&key=yt6&keepalive=yes&source=youtube&clen=4015919&pcm2=no&lmt=1449555875921501&gir=yes&upn=3Cks0aHaVpw&pl=21&expire=1492863364&id=o-AGPeW3bkX1nrk-fjCVQFZIVsUdAaHNbcsWsG0M2V8e4u&itag=171&mime=audio%2Fwebm&dur=269.098&ei=JPX6WJ3rJJegd7zqodgJ&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&signature=A383A78202B32CF3799B954DA0DBF875919E4CFF.B45576B572987FBEA731120E2682D5E612CE3354&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/171-58faf5254fc43-webm-4015919/audiostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "",
			"bitrate": "128",
			"codec": "Vorbis",
			"itag": "171",
			"vidid": "CevxZvSJLk8"
		},
		"2": {
			"rSize": "1.56 MB",
			"quality": "",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?mt=1492841663&mv=m&initcwndbps=183750&ipbits=0&ms=au&mm=31&mn=sn-5uh5o-f5f6&ip=137.74.1.176&key=yt6&keepalive=yes&source=youtube&clen=1637862&pcm2=no&lmt=1449555874424077&gir=yes&upn=3Cks0aHaVpw&pl=21&expire=1492863364&id=o-AGPeW3bkX1nrk-fjCVQFZIVsUdAaHNbcsWsG0M2V8e4u&itag=249&mime=audio%2Fwebm&dur=269.121&ei=JPX6WJ3rJJegd7zqodgJ&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&signature=B99461AC678080521E516D1AB93E61D9A9CB1DEB.D2EE6D4117F3EE066A73CE0124E36EBDEDEE9D8C&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/249-58faf5254fc43-webm-1637862/audiostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "",
			"bitrate": "48",
			"codec": "Opus",
			"itag": "249",
			"vidid": "CevxZvSJLk8"
		},
		"3": {
			"rSize": "2.04 MB",
			"quality": "",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?mt=1492841663&mv=m&initcwndbps=183750&ipbits=0&ms=au&mm=31&mn=sn-5uh5o-f5f6&ip=137.74.1.176&key=yt6&keepalive=yes&source=youtube&clen=2137068&pcm2=no&lmt=1449555875441543&gir=yes&upn=3Cks0aHaVpw&pl=21&expire=1492863364&id=o-AGPeW3bkX1nrk-fjCVQFZIVsUdAaHNbcsWsG0M2V8e4u&itag=250&mime=audio%2Fwebm&dur=269.121&ei=JPX6WJ3rJJegd7zqodgJ&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&signature=06CD7B4B370845B7F55BB784F13EB76B9B853D3E.0D5E87A668E790C98573C96E9F56AEF7C6071002&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/250-58faf5254fc43-webm-2137068/audiostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "",
			"bitrate": "64",
			"codec": "Opus",
			"itag": "250",
			"vidid": "CevxZvSJLk8"
		},
		"4": {
			"rSize": "4.04 MB",
			"quality": "",
			"directurl": "https://r2---sn-5uh5o-f5f6.googlevideo.com/videoplayback?mt=1492841663&mv=m&initcwndbps=183750&ipbits=0&ms=au&mm=31&mn=sn-5uh5o-f5f6&ip=137.74.1.176&key=yt6&keepalive=yes&source=youtube&clen=4235503&pcm2=no&lmt=1449555873227770&gir=yes&upn=3Cks0aHaVpw&pl=21&expire=1492863364&id=o-AGPeW3bkX1nrk-fjCVQFZIVsUdAaHNbcsWsG0M2V8e4u&itag=251&mime=audio%2Fwebm&dur=269.121&ei=JPX6WJ3rJJegd7zqodgJ&requiressl=yes&sparams=clen%2Cdur%2Cei%2Cgir%2Cid%2Cinitcwndbps%2Cip%2Cipbits%2Citag%2Ckeepalive%2Clmt%2Cmime%2Cmm%2Cmn%2Cms%2Cmv%2Cpcm2%2Cpl%2Crequiressl%2Csource%2Cupn%2Cexpire&signature=CB151F0C7872AA59F15613AAB82020AEEDABF196.0C5BA6371382B6346348FB4725B2DB7397127C99&ratebypass=yes",
			"dloadUrl": "//video.download-lagu-mp3.com/@download/251-58faf5254fc43-webm-4235503/audiostreams/CevxZvSJLk8/Katy%2BPerry%2B-%2BRoar%2B%2528Official%2529.webm",
			"ftype": "webm",
			"framerate": "",
			"bitrate": "160",
			"codec": "Opus",
			"itag": "251",
			"vidid": "CevxZvSJLk8"
		}
	}
}</pre>
</div>
</div>
</div>
