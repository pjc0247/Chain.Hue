# Chain.Hue
Philipse Hue

```cs
C.EventSource<SlackMessage>()
  .Filter<MessageRegex>("LIGHT ON") /* SOME FILTER */
  .Task<TurnOnLight>(1);
```

처음 실행할 경우
----
```cs
.Task<GetAppKey>()
```
```cs
.Task<EnumLights>()
```

Tasks
----
__TurnOnLight__
```cs
.Task<TurnOnLight>("LIGHT_ID")
```
__TurnOffLight__
```cs
.Task<TurnOffLight>("LIGHT_ID")
```
__SetBrightness__
```cs
.Task<SetBrightness>("LIGHT_ID", 0 ~ 255)
```
__SetColor__
```cs
.Task<SetColor>("LIGHT_ID", R, G, B)
```

Setup Hue API
----
http://pjc0247.tistory.com/78
