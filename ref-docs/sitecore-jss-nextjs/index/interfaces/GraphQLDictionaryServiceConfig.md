[**@sitecore-jss/sitecore-jss-nextjs**](../../README.md) • **Docs**

***

[@sitecore-jss/sitecore-jss-nextjs](../../README.md) / [index](../README.md) / GraphQLDictionaryServiceConfig

# Interface: GraphQLDictionaryServiceConfig

Configuration options for

## See

GraphQLDictionaryService instances

## Extends

- `Omit`\<`SearchQueryVariables`, `"language"`\>.[`CacheOptions`](CacheOptions.md).`Pick`\<`GraphQLRequestClientConfig`, `"retries"` \| `"retryStrategy"`\>

## Properties

### cacheEnabled?

> `optional` **cacheEnabled**: `boolean`

Enable/disable caching mechanism

#### Default

```ts
true
```

#### Inherited from

[`CacheOptions`](CacheOptions.md).[`cacheEnabled`](CacheOptions.md#cacheenabled)

#### Defined in

sitecore-jss/types/cache-client.d.ts:28

***

### cacheTimeout?

> `optional` **cacheTimeout**: `number`

Cache timeout (sec)

#### Default

```ts
60
```

#### Inherited from

[`CacheOptions`](CacheOptions.md).[`cacheTimeout`](CacheOptions.md#cachetimeout)

#### Defined in

sitecore-jss/types/cache-client.d.ts:33

***

### clientFactory

> **clientFactory**: [`GraphQLRequestClientFactory`](../../graphql/type-aliases/GraphQLRequestClientFactory.md)

A GraphQL Request Client Factory is a function that accepts configuration and returns an instance of a GraphQLRequestClient.
This factory function is used to create and configure GraphQL clients for making GraphQL API requests.

#### Defined in

sitecore-jss/types/i18n/graphql-dictionary-service.d.ts:20

***

### dictionaryEntryTemplateId?

> `optional` **dictionaryEntryTemplateId**: `string`

Optional. The template ID to use when searching for dictionary entries.

#### Default

```ts
'6d1cd89719364a3aa511289a94c2a7b1' (/sitecore/templates/System/Dictionary/Dictionary entry)
```

#### Defined in

sitecore-jss/types/i18n/graphql-dictionary-service.d.ts:25

***

### jssAppTemplateId?

> `optional` **jssAppTemplateId**: `string`

Optional. The template ID of a JSS App to use when searching for the appRootId.

#### Default

```ts
'061cba1554744b918a0617903b102b82' (/sitecore/templates/Foundation/JavaScript Services/App)
```

#### Defined in

sitecore-jss/types/i18n/graphql-dictionary-service.d.ts:30

***

### pageSize?

> `optional` **pageSize**: `number`

common variable for all GraphQL queries
it will be used for every type of query to regulate result batch size
Optional. How many result items to fetch in each GraphQL call. This is needed for pagination.

#### Default

```ts
10
```

#### Inherited from

`Omit.pageSize`

#### Defined in

sitecore-jss/types/graphql/search-service.d.ts:52

***

### retries?

> `optional` **retries**: `number`

Number of retries for client. Will use the specified `retryStrategy`.

#### Inherited from

`Pick.retries`

#### Defined in

sitecore-jss/types/graphql-request-client.d.ts:74

***

### retryStrategy?

> `optional` **retryStrategy**: [`RetryStrategy`](../../graphql/interfaces/RetryStrategy.md)

Retry strategy for the client. Uses `DefaultRetryStrategy` by default with exponential
back-off factor of 2 for codes 429, 502, 503, 504, 520, 521, 522, 523, 524.

#### Inherited from

`Pick.retryStrategy`

#### Defined in

sitecore-jss/types/graphql-request-client.d.ts:79

***

### rootItemId?

> `optional` **rootItemId**: `string`

Optional. The ID of the search root item. Fetch items that have this item as an ancestor.

#### Inherited from

`Omit.rootItemId`

#### Defined in

sitecore-jss/types/graphql/search-service.d.ts:41

***

### siteName

> **siteName**: `string`

The name of the current Sitecore site. This is used to to determine the search query root
in cases where one is not specified by the caller.

#### Defined in

sitecore-jss/types/i18n/graphql-dictionary-service.d.ts:15

***

### templates?

> `optional` **templates**: `string`

Optional. Sitecore template ID(s). Fetch items that inherit from this template(s).

#### Inherited from

`Omit.templates`

#### Defined in

sitecore-jss/types/graphql/search-service.d.ts:45

***

### useSiteQuery?

> `optional` **useSiteQuery**: `boolean`

Optional. Use site query for dictionary fetch instead of search query (XM Cloud only)

#### Defined in

sitecore-jss/types/i18n/graphql-dictionary-service.d.ts:34
