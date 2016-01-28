<properties
	pageTitle="SaveData and LoadData functions | Microsoft PowerApps"
	description="Reference information, including syntax, for the SaveData and LoadData functions in PowerApps"
	services=""
	suite="powerapps"
	documentationCenter="na"
	authors="gregli-msft"
	manager="dwrede"
	editor=""
	tags=""/>

<tags
   ms.service="powerapps"
   ms.devlang="na"
   ms.topic="article"
   ms.tgt_pltfrm="na"
   ms.workload="na"
   ms.date="11/07/2015"
   ms.author="gregli"/>

# SaveData and LoadData functions in PowerApps #

Saves and re-loads a [collection](working-with-data-sources.md#collections).

## Description ##

The **SaveData** function stores a collection for later use under a name.  

The **LoadData** function re-loads a collection by name that was previously saved with **SaveData**. You can't use this function to load a collection from another source.  

**LoadData** doesn't create the collection; the function only fills an existing collection. You must first create the collection with the correct [columns](working-with-tables.md#columns) by using **[Collect](function-clear-collect-clearcollect.md)**.

Storage is encrypted and in a private location on the local device, isolated from other users and other apps.  

## Syntax ##

**SaveData**( *Collection*, *Name* )<br>**LoadData**( *Collection*, *Name* )

- *Collection* - Required.  Collection to be stored or loaded.
- *Name* - Required.  Name of the storage. You must use the same name to save and load the same set of data. The name space isn't shared with other apps or users.