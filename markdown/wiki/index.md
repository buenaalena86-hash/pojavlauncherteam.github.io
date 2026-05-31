javax.net.ssl.SSLHandshakeException: java.security.cert.CertPathValidatorException: Trust anchor for certification path not found.
	at com.android.org.conscrypt.ConscryptFileDescriptorSocket.startHandshake(ConscryptFileDescriptorSocket.java:231)
	at com.android.okhttp.internal.io.RealConnection.connectTls(RealConnection.java:196)
	at com.android.okhttp.internal.io.RealConnection.connectSocket(RealConnection.java:153)
	at com.android.okhttp.internal.io.RealConnection.connect(RealConnection.java:116)
	at com.android.okhttp.internal.http.StreamAllocation.findConnection(StreamAllocation.java:186)
	at com.android.okhttp.internal.http.StreamAllocation.findHealthyConnection(StreamAllocation.java:128)
	at com.android.okhttp.internal.http.StreamAllocation.newStream(StreamAllocation.java:97)
	at com.android.okhttp.internal.http.HttpEngine.connect(HttpEngine.java:302)
	at com.android.okhttp.internal.http.HttpEngine.sendRequest(HttpEngine.java:245)
	at com.android.okhttp.internal.huc.HttpURLConnectionImpl.execute(HttpURLConnectionImpl.java:465)
	at com.android.okhttp.internal.huc.HttpURLConnectionImpl.getResponse(HttpURLConnectionImpl.java:411)
	at com.android.okhttp.internal.huc.HttpURLConnectionImpl.getInputStream(HttpURLConnectionImpl.java:248)
	at com.android.okhttp.internal.huc.DelegatingHttpsURLConnection.getInputStream(DelegatingHttpsURLConnection.java:211)
	at com.android.okhttp.internal.huc.HttpsURLConnectionImpl.getInputStream(HttpsURLConnectionImpl.java:30)
	at net.kdt.pojavlaunch.utils.DownloadUtils.downloadFileMonitored(DownloadUtils.java:70)
	at net.kdt.pojavlaunch.mirrors.DownloadMirror.downloadFileMirrored(DownloadMirror.java:41)
	at net.kdt.pojavlaunch.tasks.MinecraftDownloader$DownloaderTask.lambda$downloadFile$0$net-kdt-pojavlaunch-tasks-MinecraftDownloader$DownloaderTask(MinecraftDownloader.java:469)
	at net.kdt.pojavlaunch.tasks.MinecraftDownloader$DownloaderTask$$ExternalSyntheticLambda0.call(D8$$SyntheticClass:0)
	at net.kdt.pojavlaunch.utils.DownloadUtils.downloadFile(DownloadUtils.java:125)
	at net.kdt.pojavlaunch.utils.DownloadUtils.ensureSha1(DownloadUtils.java:151)
	at net.kdt.pojavlaunch.tasks.MinecraftDownloader$DownloaderTask.downloadFile(MinecraftDownloader.java:468)
	at net.kdt.pojavlaunch.tasks.MinecraftDownloader$DownloaderTask.verifyFileSha1(MinecraftDownloader.java:462)
	at net.kdt.pojavlaunch.tasks.MinecraftDownloader$DownloaderTask.runCatching(MinecraftDownloader.java:447)
	at net.kdt.pojavlaunch.tasks.MinecraftDownloader$DownloaderTask.run(MinecraftDownloader.java:435)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
	at java.lang.Thread.run(Thread.java:919)
Caused by: java.security.cert.CertificateException: java.security.cert.CertPathValidatorException: Trust anchor for certification path not found.
	at com.android.org.conscrypt.TrustManagerImpl.verifyChain(TrustManagerImpl.java:674)
	at com.android.org.conscrypt.TrustManagerImpl.checkTrustedRecursive(TrustManagerImpl.java:551)
	at com.android.org.conscrypt.TrustManagerImpl.checkTrustedRecursive(TrustManagerImpl.java:617)
	at com.android.org.conscrypt.TrustManagerImpl.checkTrustedRecursive(TrustManagerImpl.java:640)
	at com.android.org.conscrypt.TrustManagerImpl.checkTrustedRecursive(TrustManagerImpl.java:640)
	at com.android.org.conscrypt.TrustManagerImpl.checkTrusted(TrustManagerImpl.java:507)
	at com.android.org.conscrypt.TrustManagerImpl.checkTrusted(TrustManagerImpl.java:426)
	at com.android.org.conscrypt.TrustManagerImpl.getTrustedChainForServer(TrustManagerImpl.java:354)
	at android.security.net.config.NetworkSecurityTrustManager.checkServerTrusted(NetworkSecurityTrustManager.java:94)
	at android.security.net.config.RootTrustManager.checkServerTrusted(RootTrustManager.java:89)
	at com.android.org.conscrypt.Platform.checkServerTrusted(Platform.java:224)
	at com.android.org.conscrypt.ConscryptFileDescriptorSocket.verifyCertificateChain(ConscryptFileDescriptorSocket.java:407)
	at com.android.org.conscrypt.NativeCrypto.SSL_do_handshake(Native Method)
	at com.android.org.conscrypt.NativeSsl.doHandshake(NativeSsl.java:387)
	at com.android.org.conscrypt.ConscryptFileDescriptorSocket.startHandshake(ConscryptFileDescriptorSocket.java:226)
	... 26 more
Caused by: java.security.cert.CertPathValidatorException: Trust anchor for certification path not found.
	... 41 more
  
# Welcome to the PojavLauncher Wiki!
____
* Get started by [installing Pojavlauncher](./getting_started/INSTALL)!
* Got a question? Check out our [FAQ](./faq/INSTALLATIONOFMODSRPWORLDS)!
* Wanna contribute to the project? [Look here](../contribute/CONT-WEBSITE.md)

