# wls-log4j-jdk8

A do-nothing Java web application to demonstrate what happens when WebLogic 12.x, running on Java 8, encounters
a multi-release jar in `WEB-INF/lib`.

Une application bidon Web Java pour montrer ce qui se passe lorsque WebLogic 12.x, exécuté sur Java 8, rencontre
un multi-version jar dans `WEB-INF/lib`.

```
<14-Dec-2021 7:42:53 o'clock AM NST> <Warning> <Deployer> <BEA-149078> <Stack trace for message 149004
weblogic.application.ModuleException: null
null
	at weblogic.servlet.internal.WebAppModule.createModuleException(WebAppModule.java:1824)
	at weblogic.servlet.internal.WebAppModule.init(WebAppModule.java:270)
	at weblogic.servlet.internal.WebAppModule.init(WebAppModule.java:682)
	at weblogic.application.internal.flow.ScopedModuleDriver.init(ScopedModuleDriver.java:162)
	at weblogic.application.internal.ExtensibleModuleWrapper.init(ExtensibleModuleWrapper.java:98)
	Truncated. see log file for complete stacktrace
Caused By: java.lang.IllegalArgumentException
	at com.bea.objectweb.asm.ClassReader.<init>(Unknown Source)
	at com.bea.objectweb.asm.ClassReader.<init>(Unknown Source)
	at weblogic.application.utils.annotation.ClassInfoImpl.<init>(ClassInfoImpl.java:41)
	at weblogic.application.utils.annotation.ClassfinderClassInfos.polulateOneClassInfo(ClassfinderClassInfos.java:240)
	at weblogic.application.utils.annotation.ClassfinderClassInfos.populateClassInfos(ClassfinderClassInfos.java:193)
	Truncated. see log file for complete stacktrace
> 
```

## Building / Création

Import project into Eclipse; right click and *Export → WAR file*.

Importer le projet dans Eclipse; clic-droit et *Exporter → fichier WAR*.

