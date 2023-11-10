---
title: Test
seo_title: Test
summary: This is a test post.
description: 
slug: test
author: Dovydas Ciomenas

draft: true
date: 2023-11-10T15:18:27+02:00
lastmod: 
expiryDate: 
publishDate: 

feature_image: shadertoy.png
feature_image_alt: 

categories: [Test]
tags: [test]
series:

toc: false
related: true
social_share: true
newsletter: false
disable_comments: true
---

This is a test post.

```cpp
void UToonTanksGameInstance::AsyncCheckLatestVersion()
{
	auto Request = FHttpModule::Get().CreateRequest();
	Request->SetURL(FString("https://itch.io/api/1/x/wharf/latest?game_id=2318899&channel_name=windows"));
	Request->OnProcessRequestComplete().BindLambda([this](const FHttpRequestPtr& Request, const FHttpResponsePtr& Response, bool bSuccess)
	{
		if (bSuccess && Response->GetContentType() == "application/json")
		{
			TSharedPtr<FJsonObject> JsonObject = MakeShareable(new FJsonObject());

			TSharedRef<TJsonReader<TCHAR>> JsonReader = TJsonReaderFactory<TCHAR>::Create(Response->GetContentAsString());

			FJsonSerializer::Deserialize(JsonReader, JsonObject);

			ItchLatestVersion = JsonObject->GetStringField("latest");
		}
		else
		{
			UE_LOG(LogTemp, Error, TEXT("Unable to GET latest version"));
		}
	});

	Request->ProcessRequest();
}

```