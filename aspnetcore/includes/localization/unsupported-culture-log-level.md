> [!NOTE]
> 在 ASP.NET Core 3.0 之前，如果请求的区域性不受支持，Web 应用将写入每个请求的一个类型为 `LogLevel.Warning` 的日志。 记录每个请求的一个 `LogLevel.Warning` 可以生成包含冗余信息的大型日志文件。 此行为已在 ASP.NET 3.0 中进行了更改。 `RequestLocalizationMiddleware` 写入类型为 `LogLevel.Debug` 的日志，这会减小生产日志的大小。