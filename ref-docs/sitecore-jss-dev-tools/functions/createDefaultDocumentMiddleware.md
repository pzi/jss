[**@sitecore-jss/sitecore-jss-dev-tools**](../README.md) • **Docs**

***

[@sitecore-jss/sitecore-jss-dev-tools](../README.md) / createDefaultDocumentMiddleware

# Function: createDefaultDocumentMiddleware()

> **createDefaultDocumentMiddleware**(`config`): (`req`, `res`, `next`) => `void`

## Parameters

| Parameter | Type | Description |
| ------ | ------ | ------ |
| `config` | [`DefaultDocumentMiddlewareOptions`](../interfaces/DefaultDocumentMiddlewareOptions.md) |  |

## Returns

`Function`

### Parameters

| Parameter | Type |
| ------ | ------ |
| `req` | `Request`\<`ParamsDictionary`, `any`, `any`, `ParsedQs`, `Record`\<`string`, `any`\>\> |
| `res` | `Response`\<`any`, `Record`\<`string`, `any`\>\> |
| `next` | `NextFunction` |

### Returns

`void`

## Defined in

[sitecore-jss-dev-tools/src/disconnected-server/default-document.ts:14](https://github.com/Sitecore/jss/blob/d56062542bc79b861e80260c109b6674c65ef288/packages/sitecore-jss-dev-tools/src/disconnected-server/default-document.ts#L14)
