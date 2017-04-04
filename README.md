# api documentation for  [rest (v2.0.0)](https://github.com/cujojs/rest#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-rest.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rest) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rest.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rest)
#### RESTful HTTP client library

[![NPM](https://nodei.co/npm/rest.png?downloads=true)](https://www.npmjs.com/package/rest)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rest/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-rest_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rest/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rest/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rest/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "browser": "./browser",
    "bugs": {
        "url": "https://github.com/cujojs/rest/issues"
    },
    "contributors": [
        {
            "name": "Jeremy Grelle",
            "email": "jeremy.grelle@gmail.com"
        },
        {
            "name": "John Hann",
            "url": "http://unscriptable.com"
        },
        {
            "name": "Michael Jackson",
            "url": "https://github.com/mjackson"
        }
    ],
    "dependencies": {},
    "description": "RESTful HTTP client library",
    "devDependencies": {
        "curl": "https://github.com/cujojs/curl/tarball/0.7.3",
        "poly": "https://github.com/cujojs/poly/tarball/0.5.1",
        "test-support": "~0.4",
        "when": "~3",
        "wire": "~0.9"
    },
    "directories": {},
    "dist": {
        "shasum": "6dfadf66a405c49cfbd5b4bd25b59fd29cd861bc",
        "tarball": "https://registry.npmjs.org/rest/-/rest-2.0.0.tgz"
    },
    "gitHead": "4bd359df2df845eda628d2256fd06bc4a1f5009c",
    "homepage": "https://github.com/cujojs/rest#readme",
    "jspm": {
        "registry": "npm",
        "main": "./browser"
    },
    "keywords": [
        "rest",
        "http",
        "client",
        "rest-template",
        "spring",
        "cujojs"
    ],
    "license": "MIT",
    "main": "./node",
    "maintainers": [
        {
            "name": "scothis",
            "email": "scothis@gmail.com"
        }
    ],
    "name": "rest",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/cujojs/rest.git"
    },
    "scripts": {
        "buster": "buster test --node",
        "lint": "jshint .",
        "sauceme": "sauceme",
        "start": "buster static -e browser",
        "test": "npm run-script lint && npm run-script buster",
        "tunnel": "sauceme -m"
    },
    "version": "2.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module rest](#apidoc.module.rest)
1.  [function <span class="apidocSignatureSpan">rest.</span>UrlBuilder (template, params)](#apidoc.element.rest.UrlBuilder)
1.  [function <span class="apidocSignatureSpan">rest.</span>chain ()](#apidoc.element.rest.chain)
1.  [function <span class="apidocSignatureSpan">rest.</span>getDefaultClient ()](#apidoc.element.rest.getDefaultClient)
1.  [function <span class="apidocSignatureSpan">rest.</span>interceptor (handlers)](#apidoc.element.rest.interceptor)
1.  [function <span class="apidocSignatureSpan">rest.</span>jsonp (request)](#apidoc.element.rest.jsonp)
1.  [function <span class="apidocSignatureSpan">rest.</span>node (request)](#apidoc.element.rest.node)
1.  [function <span class="apidocSignatureSpan">rest.</span>resetDefaultClient ()](#apidoc.element.rest.resetDefaultClient)
1.  [function <span class="apidocSignatureSpan">rest.</span>responsePromise (obj, callback, errback)](#apidoc.element.rest.responsePromise)
1.  [function <span class="apidocSignatureSpan">rest.</span>setDefaultClient (client)](#apidoc.element.rest.setDefaultClient)
1.  [function <span class="apidocSignatureSpan">rest.</span>setPlatformDefaultClient (client)](#apidoc.element.rest.setPlatformDefaultClient)
1.  [function <span class="apidocSignatureSpan">rest.</span>wrap (interceptor, config)](#apidoc.element.rest.wrap)
1.  [function <span class="apidocSignatureSpan">rest.</span>xhr (request)](#apidoc.element.rest.xhr)
1.  object <span class="apidocSignatureSpan">rest.</span>UrlBuilder.prototype
1.  object <span class="apidocSignatureSpan">rest.</span>base64
1.  object <span class="apidocSignatureSpan">rest.</span>find
1.  object <span class="apidocSignatureSpan">rest.</span>pubsub
1.  object <span class="apidocSignatureSpan">rest.</span>registry
1.  object <span class="apidocSignatureSpan">rest.</span>rfc5988
1.  object <span class="apidocSignatureSpan">rest.</span>uriEncoder
1.  object <span class="apidocSignatureSpan">rest.</span>uriTemplate

#### [module rest.UrlBuilder](#apidoc.module.rest.UrlBuilder)
1.  [function <span class="apidocSignatureSpan">rest.</span>UrlBuilder (template, params)](#apidoc.element.rest.UrlBuilder.UrlBuilder)

#### [module rest.UrlBuilder.prototype](#apidoc.module.rest.UrlBuilder.prototype)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>append (template, params)](#apidoc.element.rest.UrlBuilder.prototype.append)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>build (params)](#apidoc.element.rest.UrlBuilder.prototype.build)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>fullyQualify ()](#apidoc.element.rest.UrlBuilder.prototype.fullyQualify)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>isAbsolute ()](#apidoc.element.rest.UrlBuilder.prototype.isAbsolute)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>isCrossOrigin ()](#apidoc.element.rest.UrlBuilder.prototype.isCrossOrigin)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>isFullyQualified ()](#apidoc.element.rest.UrlBuilder.prototype.isFullyQualified)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>parts ()](#apidoc.element.rest.UrlBuilder.prototype.parts)
1.  [function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>toString ()](#apidoc.element.rest.UrlBuilder.prototype.toString)

#### [module rest.base64](#apidoc.module.rest.base64)
1.  [function <span class="apidocSignatureSpan">rest.base64.</span>decode (text)](#apidoc.element.rest.base64.decode)
1.  [function <span class="apidocSignatureSpan">rest.base64.</span>encode (text)](#apidoc.element.rest.base64.encode)

#### [module rest.find](#apidoc.module.rest.find)
1.  [function <span class="apidocSignatureSpan">rest.find.</span>findProperties (obj, prop, callback)](#apidoc.element.rest.find.findProperties)

#### [module rest.interceptor](#apidoc.module.rest.interceptor)
1.  [function <span class="apidocSignatureSpan">rest.</span>interceptor (handlers)](#apidoc.element.rest.interceptor.interceptor)
1.  [function <span class="apidocSignatureSpan">rest.interceptor.</span>ComplexRequest (properties)](#apidoc.element.rest.interceptor.ComplexRequest)

#### [module rest.jsonp](#apidoc.module.rest.jsonp)
1.  [function <span class="apidocSignatureSpan">rest.</span>jsonp (request)](#apidoc.element.rest.jsonp.jsonp)
1.  [function <span class="apidocSignatureSpan">rest.jsonp.</span>chain ()](#apidoc.element.rest.jsonp.chain)
1.  [function <span class="apidocSignatureSpan">rest.jsonp.</span>wrap (interceptor, config)](#apidoc.element.rest.jsonp.wrap)

#### [module rest.node](#apidoc.module.rest.node)
1.  [function <span class="apidocSignatureSpan">rest.</span>node (request)](#apidoc.element.rest.node.node)
1.  [function <span class="apidocSignatureSpan">rest.node.</span>chain ()](#apidoc.element.rest.node.chain)
1.  [function <span class="apidocSignatureSpan">rest.node.</span>wrap (interceptor, config)](#apidoc.element.rest.node.wrap)

#### [module rest.pubsub](#apidoc.module.rest.pubsub)
1.  [function <span class="apidocSignatureSpan">rest.pubsub.</span>publish (topic)](#apidoc.element.rest.pubsub.publish)
1.  [function <span class="apidocSignatureSpan">rest.pubsub.</span>subscribe (topic, callback)](#apidoc.element.rest.pubsub.subscribe)

#### [module rest.registry](#apidoc.module.rest.registry)
1.  [function <span class="apidocSignatureSpan">rest.registry.</span>child ()](#apidoc.element.rest.registry.child)
1.  [function <span class="apidocSignatureSpan">rest.registry.</span>delegate (type)](#apidoc.element.rest.registry.delegate)
1.  [function <span class="apidocSignatureSpan">rest.registry.</span>lookup (type)](#apidoc.element.rest.registry.lookup)
1.  [function <span class="apidocSignatureSpan">rest.registry.</span>register (type, converter)](#apidoc.element.rest.registry.register)

#### [module rest.responsePromise](#apidoc.module.rest.responsePromise)
1.  [function <span class="apidocSignatureSpan">rest.</span>responsePromise (obj, callback, errback)](#apidoc.element.rest.responsePromise.responsePromise)
1.  [function <span class="apidocSignatureSpan">rest.responsePromise.</span>make (promise)](#apidoc.element.rest.responsePromise.make)
1.  [function <span class="apidocSignatureSpan">rest.responsePromise.</span>promise (func)](#apidoc.element.rest.responsePromise.promise)
1.  [function <span class="apidocSignatureSpan">rest.responsePromise.</span>reject (val)](#apidoc.element.rest.responsePromise.reject)

#### [module rest.rfc5988](#apidoc.module.rest.rfc5988)
1.  [function <span class="apidocSignatureSpan">rest.rfc5988.</span>SyntaxError (expected, found, offset, line, column)](#apidoc.element.rest.rfc5988.SyntaxError)
1.  [function <span class="apidocSignatureSpan">rest.rfc5988.</span>parse (input, startRule)](#apidoc.element.rest.rfc5988.parse)
1.  [function <span class="apidocSignatureSpan">rest.rfc5988.</span>toSource ()](#apidoc.element.rest.rfc5988.toSource)

#### [module rest.uriEncoder](#apidoc.module.rest.uriEncoder)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>decode (str)](#apidoc.element.rest.uriEncoder.decode)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encode (str)](#apidoc.element.rest.uriEncoder.encode)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeFragment (str)](#apidoc.element.rest.uriEncoder.encodeFragment)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeHost (str)](#apidoc.element.rest.uriEncoder.encodeHost)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodePath (str)](#apidoc.element.rest.uriEncoder.encodePath)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodePathSegment (str)](#apidoc.element.rest.uriEncoder.encodePathSegment)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodePort (str)](#apidoc.element.rest.uriEncoder.encodePort)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeQuery (str)](#apidoc.element.rest.uriEncoder.encodeQuery)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeScheme (str)](#apidoc.element.rest.uriEncoder.encodeScheme)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeURL (str)](#apidoc.element.rest.uriEncoder.encodeURL)
1.  [function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeUserInfo (str)](#apidoc.element.rest.uriEncoder.encodeUserInfo)

#### [module rest.uriTemplate](#apidoc.module.rest.uriTemplate)
1.  [function <span class="apidocSignatureSpan">rest.uriTemplate.</span>expand (template, params)](#apidoc.element.rest.uriTemplate.expand)

#### [module rest.xhr](#apidoc.module.rest.xhr)
1.  [function <span class="apidocSignatureSpan">rest.</span>xhr (request)](#apidoc.element.rest.xhr.xhr)
1.  [function <span class="apidocSignatureSpan">rest.xhr.</span>chain ()](#apidoc.element.rest.xhr.chain)
1.  [function <span class="apidocSignatureSpan">rest.xhr.</span>wrap (interceptor, config)](#apidoc.element.rest.xhr.wrap)



# <a name="apidoc.module.rest"></a>[module rest](#apidoc.module.rest)

#### <a name="apidoc.element.rest.UrlBuilder"></a>[function <span class="apidocSignatureSpan">rest.</span>UrlBuilder (template, params)](#apidoc.element.rest.UrlBuilder)
- description and source-code
```javascript
function UrlBuilder(template, params) {
	if (!(this instanceof UrlBuilder)) {
		// invoke as a constructor
		return new UrlBuilder(template, params);
	}

	if (template instanceof UrlBuilder) {
		this._template = template.template;
		this._params = mixin({}, this._params, params);
	}
	else {
		this._template = (template || '').toString();
		this._params = params || {};
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.chain"></a>[function <span class="apidocSignatureSpan">rest.</span>chain ()](#apidoc.element.rest.chain)
- description and source-code
```javascript
function chain() {
		if (typeof console !== 'undefined') {
			console.log('rest.js: client.chain() is deprecated, use client.wrap() instead');
		}

		return impl.wrap.apply(this, arguments);
	}
```
- example usage
```shell
...
1.1.1
- support for IE 11, Safari 7 and iOS 7 (no code changes required, now actively testing)
- Node specific configuration options via request.mixin. Particularly useful for https clients. Thanks @wwwdata
- basic support for Browserify. Note: Browserify is not yet a tested environment

1.1.0
- bump when.js version to ~3, 2.x is no longer supported
- perfer 'client.wrap()' to 'client.chain()', 'chain' is now deprecated
- add HTTP specific methods to the promises returned from clients: .entity(), .status(), .headers(), .header(name)
- mime converters may return a promise. Thanks @phillipj
- removed 'rest/util/beget' favor Object.create

1.0.3
- add moduleType for bower (node and amd). Thanks @briancavalier
- doc polish. Thanks @gogamoga
...
```

#### <a name="apidoc.element.rest.getDefaultClient"></a>[function <span class="apidocSignatureSpan">rest.</span>getDefaultClient ()](#apidoc.element.rest.getDefaultClient)
- description and source-code
```javascript
function getDefaultClient() {
	return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.interceptor"></a>[function <span class="apidocSignatureSpan">rest.</span>interceptor (handlers)](#apidoc.element.rest.interceptor)
- description and source-code
```javascript
function interceptor(handlers) {

	var initHandler, requestHandler, successResponseHandler, errorResponseHandler;

	handlers = handlers || {};

	initHandler            = handlers.init    || defaultInitHandler;
	requestHandler         = handlers.request || defaultRequestHandler;
	successResponseHandler = handlers.success || handlers.response || defaultResponseHandler;
	errorResponseHandler   = handlers.error   || function () {
		// Propagate the rejection, with the result of the handler
		return Promise.resolve((handlers.response || defaultResponseHandler).apply(this, arguments))
			.then(Promise.reject.bind(Promise));
	};

	return function (target, config) {

		if (typeof target === 'object') {
			config = target;
		}
		if (typeof target !== 'function') {
			target = handlers.client || defaultClient;
		}

		config = initHandler(config || {});

		function interceptedClient(request) {
			var context, meta;
			context = {};
			meta = { 'arguments': Array.prototype.slice.call(arguments), client: interceptedClient };
			request = typeof request === 'string' ? { path: request } : request || {};
			request.originator = request.originator || interceptedClient;
			return responsePromise(
				requestHandler.call(context, request, config, meta),
				function (request) {
					var response, abort, next;
					next = target;
					if (request instanceof ComplexRequest) {
						// unpack request
						abort = request.abort;
						next = request.client || next;
						response = request.response;
						// normalize request, must be last
						request = request.request;
					}
					response = response || Promise.resolve(request).then(function (request) {
						return Promise.resolve(next(request)).then(
							function (response) {
								return successResponseHandler.call(context, response, config, meta);
							},
							function (response) {
								return errorResponseHandler.call(context, response, config, meta);
							}
						);
					});
					return abort ? Promise.race([response, abort]) : response;
				},
				function (error) {
					return Promise.reject({ request: request, error: error });
				}
			);
		}

		return client(interceptedClient, target);
	};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.jsonp"></a>[function <span class="apidocSignatureSpan">rest.</span>jsonp (request)](#apidoc.element.rest.jsonp)
- description and source-code
```javascript
function jsonp(request) {
	return responsePromise.promise(function (resolve, reject) {

		var callbackName, callbackParams, script, firstScript, response;

		request = typeof request === 'string' ? { path: request } : request || {};
		response = { request: request };

		if (request.canceled) {
			response.error = 'precanceled';
			reject(response);
			return;
		}

		request.callback = request.callback || {};
		callbackName = registerCallback(request.callback.prefix || 'jsonp', resolve, response, request.callback.name);
		callbackParams = {};
		callbackParams[request.callback.param || 'callback'] = callbackName;

		request.canceled = false;
		request.cancel = function cancel() {
			request.canceled = true;
			cleanupScriptNode(response);
			reject(response);
		};

		script = document.createElement('script');
		script.type = 'text/javascript';
		script.async = true;
		script.src = response.url = new UrlBuilder(request.path, callbackParams).build();

		function handlePossibleError() {
			if (typeof window[callbackName] === 'function') {
				response.error = 'loaderror';
				clearProperty(window, callbackName);
				cleanupScriptNode(response);
				reject(response);
			}
		}
		script.onerror = function () {
			handlePossibleError();
		};
		script.onload = script.onreadystatechange = function (e) {
			// script tag load callbacks are completely non-standard
			// handle case where onreadystatechange is fired for an error instead of onerror
			if ((e && (e.type === 'load' || e.type === 'error')) || script.readyState === 'loaded') {
				handlePossibleError();
			}
		};

		response.raw = script;
		firstScript = document.getElementsByTagName('script')[0];
		firstScript.parentNode.insertBefore(script, firstScript);

	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.node"></a>[function <span class="apidocSignatureSpan">rest.</span>node (request)](#apidoc.element.rest.node)
- description and source-code
```javascript
function node(request) {
	<span class="apidocCodeCommentSpan">/*jshint maxcomplexity:20 */
</span>	return responsePromise.promise(function (resolve, reject) {

		var options, clientRequest, client, url, headers, entity, response;

		request = typeof request === 'string' ? { path: request } : request || {};
		response = { request: request };

		if (request.canceled) {
			response.error = 'precanceled';
			reject(response);
			return;
		}

		url = response.url = request.path || '';
		client = url.match(httpsExp) ? https : http;

		options = mixin({}, request.mixin, parser.parse(url));

		entity = request.entity;
		request.method = request.method || (entity ? 'POST' : 'GET');
		options.method = request.method;
		headers = options.headers = {};
		Object.keys(request.headers || {}).forEach(function (name) {
			headers[normalizeHeaderName(name)] = request.headers[name];
		});
		if (!headers['Content-Length']) {
			headers['Content-Length'] = entity ? Buffer.byteLength(entity, 'utf8') : 0;
		}

		request.canceled = false;
		request.cancel = function cancel() {
			request.canceled = true;
			clientRequest.abort();
		};

		clientRequest = client.request(options, function (clientResponse) {
			// Array of Buffers to collect response chunks
			var buffers = [];

			response.raw = {
				request: clientRequest,
				response: clientResponse
			};
			response.status = {
				code: clientResponse.statusCode
				// node doesn't provide access to the status text
			};
			response.headers = {};
			Object.keys(clientResponse.headers).forEach(function (name) {
				response.headers[normalizeHeaderName(name)] = clientResponse.headers[name];
			});

			clientResponse.on('data', function (data) {
				// Collect the next Buffer chunk
				buffers.push(data);
			});

			clientResponse.on('end', function () {
				// Create the final response entity
				response.entity = buffers.length > 0 ? Buffer.concat(buffers).toString() : '';
				buffers = null;

				resolve(response);
			});
		});

		clientRequest.on('error', function (e) {
			response.error = e;
			reject(response);
		});

		if (entity) {
			clientRequest.write(entity);
		}
		clientRequest.end();

	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.resetDefaultClient"></a>[function <span class="apidocSignatureSpan">rest.</span>resetDefaultClient ()](#apidoc.element.rest.resetDefaultClient)
- description and source-code
```javascript
function resetDefaultClient() {
	target = platformDefault;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.responsePromise"></a>[function <span class="apidocSignatureSpan">rest.</span>responsePromise (obj, callback, errback)](#apidoc.element.rest.responsePromise)
- description and source-code
```javascript
function responsePromise(obj, callback, errback) {
	return make(Promise.resolve(obj).then(callback, errback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.setDefaultClient"></a>[function <span class="apidocSignatureSpan">rest.</span>setDefaultClient (client)](#apidoc.element.rest.setDefaultClient)
- description and source-code
```javascript
function setDefaultClient(client) {
	target = client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.setPlatformDefaultClient"></a>[function <span class="apidocSignatureSpan">rest.</span>setPlatformDefaultClient (client)](#apidoc.element.rest.setPlatformDefaultClient)
- description and source-code
```javascript
function setPlatformDefaultClient(client) {
	if (platformDefault) {
		throw new Error('Unable to redefine platformDefaultClient');
	}
	target = platformDefault = client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.wrap"></a>[function <span class="apidocSignatureSpan">rest.</span>wrap (interceptor, config)](#apidoc.element.rest.wrap)
- description and source-code
```javascript
function wrap(interceptor, config) {
		return interceptor(impl, config);
	}
```
- example usage
```shell
...

'''javascript
var rest, mime, client;

rest = require('rest'),
mime = require('rest/interceptor/mime');

client = rest.wrap(mime);
client({ path: '/data.json' }).then(function(response) {
    console.log('response: ', response);
});
'''

Before an interceptor can be used, it needs to be configured.  In this case, we will accept the default configuration, and obtain
 a client.  Now when we see the response, the entity will be a JS object instead of a String.
...
```

#### <a name="apidoc.element.rest.xhr"></a>[function <span class="apidocSignatureSpan">rest.</span>xhr (request)](#apidoc.element.rest.xhr)
- description and source-code
```javascript
function xhr(request) {
	return responsePromise.promise(function (resolve, reject) {
		<span class="apidocCodeCommentSpan">/*jshint maxcomplexity:20 */
</span>
		var client, method, url, headers, entity, headerName, response, XHR;

		request = typeof request === 'string' ? { path: request } : request || {};
		response = { request: request };

		if (request.canceled) {
			response.error = 'precanceled';
			reject(response);
			return;
		}

		XHR = request.engine || XMLHttpRequest;
		if (!XHR) {
			reject({ request: request, error: 'xhr-not-available' });
			return;
		}

		entity = request.entity;
		request.method = request.method || (entity ? 'POST' : 'GET');
		method = request.method;
		url = response.url = request.path || '';

		try {
			client = response.raw = new XHR();

			// mixin extra request properties before and after opening the request as some properties require being set at different phases
 of the request
			safeMixin(client, request.mixin);
			client.open(method, url, true);
			safeMixin(client, request.mixin);

			headers = request.headers;
			for (headerName in headers) {
				/*jshint forin:false */
				if (headerName === 'Content-Type' && headers[headerName] === 'multipart/form-data') {
					// XMLHttpRequest generates its own Content-Type header with the
					// appropriate multipart boundary when sending multipart/form-data.
					continue;
				}

				client.setRequestHeader(headerName, headers[headerName]);
			}

			request.canceled = false;
			request.cancel = function cancel() {
				request.canceled = true;
				client.abort();
				reject(response);
			};

			client.onreadystatechange = function (/* e */) {
				if (request.canceled) { return; }
				if (client.readyState === (XHR.DONE || 4)) {
					response.status = {
						code: client.status,
						text: client.statusText
					};
					response.headers = parseHeaders(client.getAllResponseHeaders());
					response.entity = client.responseText;

					// #125 -- Sometimes IE8-9 uses 1223 instead of 204
					// http://stackoverflow.com/questions/10046972/msie-returns-status-code-of-1223-for-ajax-request
					if (response.status.code === 1223) {
						response.status.code = 204;
					}

					if (response.status.code > 0) {
						// check status code as readystatechange fires before error event
						resolve(response);
					}
					else {
						// give the error callback a chance to fire before resolving
						// requests for file:// URLs do not have a status code
						setTimeout(function () {
							resolve(response);
						}, 0);
					}
				}
			};

			try {
				client.onerror = function (/* e */) {
					response.error = 'loaderror';
					reject(response);
				};
			}
			catch (e) {
				// IE 6 will not support error handling
			}

			client.send(entity);
		}
		catch (e) {
			response.error = 'loaderror';
			reject(response);
		}

	});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rest.UrlBuilder"></a>[module rest.UrlBuilder](#apidoc.module.rest.UrlBuilder)

#### <a name="apidoc.element.rest.UrlBuilder.UrlBuilder"></a>[function <span class="apidocSignatureSpan">rest.</span>UrlBuilder (template, params)](#apidoc.element.rest.UrlBuilder.UrlBuilder)
- description and source-code
```javascript
function UrlBuilder(template, params) {
	if (!(this instanceof UrlBuilder)) {
		// invoke as a constructor
		return new UrlBuilder(template, params);
	}

	if (template instanceof UrlBuilder) {
		this._template = template.template;
		this._params = mixin({}, this._params, params);
	}
	else {
		this._template = (template || '').toString();
		this._params = params || {};
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rest.UrlBuilder.prototype"></a>[module rest.UrlBuilder.prototype](#apidoc.module.rest.UrlBuilder.prototype)

#### <a name="apidoc.element.rest.UrlBuilder.prototype.append"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>append (template, params)](#apidoc.element.rest.UrlBuilder.prototype.append)
- description and source-code
```javascript
append = function (template, params) {
		// TODO consider query strings and fragments
		return new UrlBuilder(this._template + template, mixin({}, this._params, params));
	}
```
- example usage
```shell
...
	},
	request: function (request, config) {
		var path, params;

		path = request.path || '';
		params = request.params || {};

		request.path = new UrlBuilder(path, config.params).append('', params).build();
		delete request.params;

		return request;
	}
});
...
```

#### <a name="apidoc.element.rest.UrlBuilder.prototype.build"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>build (params)](#apidoc.element.rest.UrlBuilder.prototype.build)
- description and source-code
```javascript
build = function (params) {
		return buildUrl(this._template, mixin({}, this._params, params));
	}
```
- example usage
```shell
...

	/**
	 * True if the URL is absolute
	 *
	 * @return {boolean}
	 */
	isAbsolute: function () {
		return absoluteUrlRE.test(this.build());
	},

	/**
	 * True if the URL is fully qualified
	 *
	 * @return {boolean}
	 */
...
```

#### <a name="apidoc.element.rest.UrlBuilder.prototype.fullyQualify"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>fullyQualify ()](#apidoc.element.rest.UrlBuilder.prototype.fullyQualify)
- description and source-code
```javascript
fullyQualify = function () {
		if (typeof location === 'undefined') { return this; }
		if (this.isFullyQualified()) { return this; }

		var template = this._template;

		if (startsWith(template, '//')) {
			template = origin.protocol + template;
		}
		else if (startsWith(template, '/')) {
			template = origin.origin + template;
		}
		else if (!this.isAbsolute()) {
			template = origin.origin + origin.pathname.substring(0, origin.pathname.lastIndexOf('/') + 1);
		}

		if (template.indexOf('/', 8) === -1) {
			// default the pathname to '/'
			template = template + '/';
		}

		return new UrlBuilder(template, this._params);
	}
```
- example usage
```shell
...
	 * @see https://developer.mozilla.org/en-US/docs/DOM/window.location
	 *
	 * @returns {Object} a 'window.location'-like object
	 */
	parts: function () {
		/*jshint maxcomplexity:20 */
		var url, parts;
		url = this.fullyQualify().build().match(urlRE);
		parts = {
			href: url[0],
			protocol: url[1],
			host: url[3] || '',
			hostname: url[4] || '',
			port: url[6],
			pathname: url[7] || '',
...
```

#### <a name="apidoc.element.rest.UrlBuilder.prototype.isAbsolute"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>isAbsolute ()](#apidoc.element.rest.UrlBuilder.prototype.isAbsolute)
- description and source-code
```javascript
isAbsolute = function () {
		return absoluteUrlRE.test(this.build());
	}
```
- example usage
```shell
...

		if (startsWith(template, '//')) {
			template = origin.protocol + template;
		}
		else if (startsWith(template, '/')) {
			template = origin.origin + template;
		}
		else if (!this.isAbsolute()) {
			template = origin.origin + origin.pathname.substring(0, origin.pathname.lastIndexOf('/') + 1);
		}

		if (template.indexOf('/', 8) === -1) {
			// default the pathname to '/'
			template = template + '/';
		}
...
```

#### <a name="apidoc.element.rest.UrlBuilder.prototype.isCrossOrigin"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>isCrossOrigin ()](#apidoc.element.rest.UrlBuilder.prototype.isCrossOrigin)
- description and source-code
```javascript
isCrossOrigin = function () {
		if (!origin) {
			return true;
		}
		var url = this.parts();
		return url.protocol !== origin.protocol ||
		       url.hostname !== origin.hostname ||
		       url.port !== origin.port;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.UrlBuilder.prototype.isFullyQualified"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>isFullyQualified ()](#apidoc.element.rest.UrlBuilder.prototype.isFullyQualified)
- description and source-code
```javascript
isFullyQualified = function () {
		return fullyQualifiedUrlRE.test(this.build());
	}
```
- example usage
```shell
...
	 *
	 * *Browser only*
	 *
	 * @return {UrlBuilder} the fully qualified URL template
	 */
	fullyQualify: function () {
		if (typeof location === 'undefined') { return this; }
		if (this.isFullyQualified()) { return this; }

		var template = this._template;

		if (startsWith(template, '//')) {
			template = origin.protocol + template;
		}
		else if (startsWith(template, '/')) {
...
```

#### <a name="apidoc.element.rest.UrlBuilder.prototype.parts"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>parts ()](#apidoc.element.rest.UrlBuilder.prototype.parts)
- description and source-code
```javascript
parts = function () {
		<span class="apidocCodeCommentSpan">/*jshint maxcomplexity:20 */
</span>		var url, parts;
		url = this.fullyQualify().build().match(urlRE);
		parts = {
			href: url[0],
			protocol: url[1],
			host: url[3] || '',
			hostname: url[4] || '',
			port: url[6],
			pathname: url[7] || '',
			search: url[8] || '',
			hash: url[9] || ''
		};
		parts.origin = parts.protocol + '//' + parts.host;
		parts.port = parts.port || (parts.protocol === 'https:' ? '443' : parts.protocol === 'http:' ? '80' : '');
		return parts;
	}
```
- example usage
```shell
...
	 *
	 * @return {boolean}
	 */
	isCrossOrigin: function () {
		if (!origin) {
			return true;
		}
		var url = this.parts();
		return url.protocol !== origin.protocol ||
		       url.hostname !== origin.hostname ||
		       url.port !== origin.port;
	},

	/**
	 * Split a URL into its consituent parts following the naming convention of
...
```

#### <a name="apidoc.element.rest.UrlBuilder.prototype.toString"></a>[function <span class="apidocSignatureSpan">rest.UrlBuilder.prototype.</span>toString ()](#apidoc.element.rest.UrlBuilder.prototype.toString)
- description and source-code
```javascript
toString = function () {
		return this.build();
	}
```
- example usage
```shell
...
	}

	if (template instanceof UrlBuilder) {
		this._template = template.template;
		this._params = mixin({}, this._params, params);
	}
	else {
		this._template = (template || '').toString();
		this._params = params || {};
	}
}

UrlBuilder.prototype = {

	/**
...
```



# <a name="apidoc.module.rest.base64"></a>[module rest.base64](#apidoc.module.rest.base64)

#### <a name="apidoc.element.rest.base64.decode"></a>[function <span class="apidocSignatureSpan">rest.base64.</span>decode (text)](#apidoc.element.rest.base64.decode)
- description and source-code
```javascript
function base64Decode(text) {

	//ignore white space
	text = text.replace(/\s/g, '');

	//first check for any unexpected input
	if (!(/^[a-z0-9\+\/\s]+\={0,2}$/i.test(text)) || text.length % 4 > 0) {
		throw new Error('Not a base64-encoded string.');
	}

	//local variables
	var cur, prev, digitNum,
		i = 0,
		result = [];

	//remove any equals signs
	text = text.replace(/\=/g, '');

	//loop over each character
	while (i < text.length) {

		cur = digits.indexOf(text.charAt(i));
		digitNum = i % 4;

		switch (digitNum) {

		//case 0: first digit - do nothing, not enough info to work with

		case 1: //second digit
			result.push(String.fromCharCode(prev << 2 | cur >> 4));
			break;

		case 2: //third digit
			result.push(String.fromCharCode((prev & 0x0f) << 4 | cur >> 2));
			break;

		case 3: //fourth digit
			result.push(String.fromCharCode((prev & 3) << 6 | cur));
			break;
		}

		prev = cur;
		i += 1;
	}

	//return a string
	return result.join('');

}
```
- example usage
```shell
...
		}
		if (prefixRE.test(variable)) {
			var prefix = prefixRE.exec(variable);
			variable = prefix[1];
			opts.maxLength = parseInt(prefix[2]);
		}

		variable = uriEncoder.decode(variable);
		value = params[variable];

		if (value === void 0 || value === null) {
			return result;
		}
		if (Array.isArray(value)) {
			result = value.reduce(function (result, value) {
...
```

#### <a name="apidoc.element.rest.base64.encode"></a>[function <span class="apidocSignatureSpan">rest.base64.</span>encode (text)](#apidoc.element.rest.base64.encode)
- description and source-code
```javascript
function base64Encode(text) {

	if (/([^\u0000-\u00ff])/.test(text)) {
		throw new Error('Can\'t base64 encode non-ASCII characters.');
	}

	var i = 0,
		cur, prev, byteNum,
		result = [];

	while (i < text.length) {

		cur = text.charCodeAt(i);
		byteNum = i % 3;

		switch (byteNum) {
		case 0: //first byte
			result.push(digits.charAt(cur >> 2));
			break;

		case 1: //second byte
			result.push(digits.charAt((prev & 3) << 4 | (cur >> 4)));
			break;

		case 2: //third byte
			result.push(digits.charAt((prev & 0x0f) << 2 | (cur >> 6)));
			result.push(digits.charAt(cur & 0x3f));
			break;
		}

		prev = cur;
		i += 1;
	}

	if (byteNum === 0) {
		result.push(digits.charAt((prev & 3) << 4));
		result.push('==');
	} else if (byteNum === 1) {
		result.push(digits.charAt((prev & 0x0f) << 2));
		result.push('=');
	}

	return result.join('');
}
```
- example usage
```shell
...
		var headers, username, password;

		headers = request.headers || (request.headers = {});
		username = request.username || config.username;
		password = request.password || config.password || '';

		if (username) {
			headers.Authorization = 'Basic ' + base64.encode(username + ':' + password);
		}

		return request;
	}
});
...
```



# <a name="apidoc.module.rest.find"></a>[module rest.find](#apidoc.module.rest.find)

#### <a name="apidoc.element.rest.find.findProperties"></a>[function <span class="apidocSignatureSpan">rest.find.</span>findProperties (obj, prop, callback)](#apidoc.element.rest.find.findProperties)
- description and source-code
```javascript
function findProperties(obj, prop, callback) {
		if (typeof obj !== 'object' || obj === null) { return; }
		if (prop in obj) {
			callback(obj[prop], obj, prop);
		}
		Object.keys(obj).forEach(function (key) {
			findProperties(obj[key], prop, callback);
		});
	}
```
- example usage
```shell
...
		}

		if (response.headers && response.headers.Link) {
			response.links = response.links || {};
			apply(response.links, parseLinkHeaders(response.headers.Link));
		}

		find.findProperties(response.entity, 'links', function (obj, host) {
			var target;

			if (Array.isArray(host.links)) {
				if (config.target === '') {
					target = host;
				}
				else {
...
```



# <a name="apidoc.module.rest.interceptor"></a>[module rest.interceptor](#apidoc.module.rest.interceptor)

#### <a name="apidoc.element.rest.interceptor.interceptor"></a>[function <span class="apidocSignatureSpan">rest.</span>interceptor (handlers)](#apidoc.element.rest.interceptor.interceptor)
- description and source-code
```javascript
function interceptor(handlers) {

	var initHandler, requestHandler, successResponseHandler, errorResponseHandler;

	handlers = handlers || {};

	initHandler            = handlers.init    || defaultInitHandler;
	requestHandler         = handlers.request || defaultRequestHandler;
	successResponseHandler = handlers.success || handlers.response || defaultResponseHandler;
	errorResponseHandler   = handlers.error   || function () {
		// Propagate the rejection, with the result of the handler
		return Promise.resolve((handlers.response || defaultResponseHandler).apply(this, arguments))
			.then(Promise.reject.bind(Promise));
	};

	return function (target, config) {

		if (typeof target === 'object') {
			config = target;
		}
		if (typeof target !== 'function') {
			target = handlers.client || defaultClient;
		}

		config = initHandler(config || {});

		function interceptedClient(request) {
			var context, meta;
			context = {};
			meta = { 'arguments': Array.prototype.slice.call(arguments), client: interceptedClient };
			request = typeof request === 'string' ? { path: request } : request || {};
			request.originator = request.originator || interceptedClient;
			return responsePromise(
				requestHandler.call(context, request, config, meta),
				function (request) {
					var response, abort, next;
					next = target;
					if (request instanceof ComplexRequest) {
						// unpack request
						abort = request.abort;
						next = request.client || next;
						response = request.response;
						// normalize request, must be last
						request = request.request;
					}
					response = response || Promise.resolve(request).then(function (request) {
						return Promise.resolve(next(request)).then(
							function (response) {
								return successResponseHandler.call(context, response, config, meta);
							},
							function (response) {
								return errorResponseHandler.call(context, response, config, meta);
							}
						);
					});
					return abort ? Promise.race([response, abort]) : response;
				},
				function (error) {
					return Promise.reject({ request: request, error: error });
				}
			);
		}

		return client(interceptedClient, target);
	};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.interceptor.ComplexRequest"></a>[function <span class="apidocSignatureSpan">rest.interceptor.</span>ComplexRequest (properties)](#apidoc.element.rest.interceptor.ComplexRequest)
- description and source-code
```javascript
function ComplexRequest(properties) {
	if (!(this instanceof ComplexRequest)) {
		// in case users forget the 'new' don't mix into the interceptor
		return new ComplexRequest(properties);
	}
	mixin(this, properties);
}
```
- example usage
```shell
...
					request.canceled = false;
				}
			}
			else if (!transient) {
				request.canceled = true;
			}
		}, timeout);
		return new interceptor.ComplexRequest({ request: request, abort: abort });
	},
	response: function (response) {
		if (this.timeout) {
			clearTimeout(this.timeout);
			delete this.timeout;
		}
		return response;
...
```



# <a name="apidoc.module.rest.jsonp"></a>[module rest.jsonp](#apidoc.module.rest.jsonp)

#### <a name="apidoc.element.rest.jsonp.jsonp"></a>[function <span class="apidocSignatureSpan">rest.</span>jsonp (request)](#apidoc.element.rest.jsonp.jsonp)
- description and source-code
```javascript
function jsonp(request) {
	return responsePromise.promise(function (resolve, reject) {

		var callbackName, callbackParams, script, firstScript, response;

		request = typeof request === 'string' ? { path: request } : request || {};
		response = { request: request };

		if (request.canceled) {
			response.error = 'precanceled';
			reject(response);
			return;
		}

		request.callback = request.callback || {};
		callbackName = registerCallback(request.callback.prefix || 'jsonp', resolve, response, request.callback.name);
		callbackParams = {};
		callbackParams[request.callback.param || 'callback'] = callbackName;

		request.canceled = false;
		request.cancel = function cancel() {
			request.canceled = true;
			cleanupScriptNode(response);
			reject(response);
		};

		script = document.createElement('script');
		script.type = 'text/javascript';
		script.async = true;
		script.src = response.url = new UrlBuilder(request.path, callbackParams).build();

		function handlePossibleError() {
			if (typeof window[callbackName] === 'function') {
				response.error = 'loaderror';
				clearProperty(window, callbackName);
				cleanupScriptNode(response);
				reject(response);
			}
		}
		script.onerror = function () {
			handlePossibleError();
		};
		script.onload = script.onreadystatechange = function (e) {
			// script tag load callbacks are completely non-standard
			// handle case where onreadystatechange is fired for an error instead of onerror
			if ((e && (e.type === 'load' || e.type === 'error')) || script.readyState === 'loaded') {
				handlePossibleError();
			}
		};

		response.raw = script;
		firstScript = document.getElementsByTagName('script')[0];
		firstScript.parentNode.insertBefore(script, firstScript);

	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.jsonp.chain"></a>[function <span class="apidocSignatureSpan">rest.jsonp.</span>chain ()](#apidoc.element.rest.jsonp.chain)
- description and source-code
```javascript
function chain() {
		if (typeof console !== 'undefined') {
			console.log('rest.js: client.chain() is deprecated, use client.wrap() instead');
		}

		return impl.wrap.apply(this, arguments);
	}
```
- example usage
```shell
...
1.1.1
- support for IE 11, Safari 7 and iOS 7 (no code changes required, now actively testing)
- Node specific configuration options via request.mixin. Particularly useful for https clients. Thanks @wwwdata
- basic support for Browserify. Note: Browserify is not yet a tested environment

1.1.0
- bump when.js version to ~3, 2.x is no longer supported
- perfer 'client.wrap()' to 'client.chain()', 'chain' is now deprecated
- add HTTP specific methods to the promises returned from clients: .entity(), .status(), .headers(), .header(name)
- mime converters may return a promise. Thanks @phillipj
- removed 'rest/util/beget' favor Object.create

1.0.3
- add moduleType for bower (node and amd). Thanks @briancavalier
- doc polish. Thanks @gogamoga
...
```

#### <a name="apidoc.element.rest.jsonp.wrap"></a>[function <span class="apidocSignatureSpan">rest.jsonp.</span>wrap (interceptor, config)](#apidoc.element.rest.jsonp.wrap)
- description and source-code
```javascript
function wrap(interceptor, config) {
		return interceptor(impl, config);
	}
```
- example usage
```shell
...

'''javascript
var rest, mime, client;

rest = require('rest'),
mime = require('rest/interceptor/mime');

client = rest.wrap(mime);
client({ path: '/data.json' }).then(function(response) {
    console.log('response: ', response);
});
'''

Before an interceptor can be used, it needs to be configured.  In this case, we will accept the default configuration, and obtain
 a client.  Now when we see the response, the entity will be a JS object instead of a String.
...
```



# <a name="apidoc.module.rest.node"></a>[module rest.node](#apidoc.module.rest.node)

#### <a name="apidoc.element.rest.node.node"></a>[function <span class="apidocSignatureSpan">rest.</span>node (request)](#apidoc.element.rest.node.node)
- description and source-code
```javascript
function node(request) {
	<span class="apidocCodeCommentSpan">/*jshint maxcomplexity:20 */
</span>	return responsePromise.promise(function (resolve, reject) {

		var options, clientRequest, client, url, headers, entity, response;

		request = typeof request === 'string' ? { path: request } : request || {};
		response = { request: request };

		if (request.canceled) {
			response.error = 'precanceled';
			reject(response);
			return;
		}

		url = response.url = request.path || '';
		client = url.match(httpsExp) ? https : http;

		options = mixin({}, request.mixin, parser.parse(url));

		entity = request.entity;
		request.method = request.method || (entity ? 'POST' : 'GET');
		options.method = request.method;
		headers = options.headers = {};
		Object.keys(request.headers || {}).forEach(function (name) {
			headers[normalizeHeaderName(name)] = request.headers[name];
		});
		if (!headers['Content-Length']) {
			headers['Content-Length'] = entity ? Buffer.byteLength(entity, 'utf8') : 0;
		}

		request.canceled = false;
		request.cancel = function cancel() {
			request.canceled = true;
			clientRequest.abort();
		};

		clientRequest = client.request(options, function (clientResponse) {
			// Array of Buffers to collect response chunks
			var buffers = [];

			response.raw = {
				request: clientRequest,
				response: clientResponse
			};
			response.status = {
				code: clientResponse.statusCode
				// node doesn't provide access to the status text
			};
			response.headers = {};
			Object.keys(clientResponse.headers).forEach(function (name) {
				response.headers[normalizeHeaderName(name)] = clientResponse.headers[name];
			});

			clientResponse.on('data', function (data) {
				// Collect the next Buffer chunk
				buffers.push(data);
			});

			clientResponse.on('end', function () {
				// Create the final response entity
				response.entity = buffers.length > 0 ? Buffer.concat(buffers).toString() : '';
				buffers = null;

				resolve(response);
			});
		});

		clientRequest.on('error', function (e) {
			response.error = e;
			reject(response);
		});

		if (entity) {
			clientRequest.write(entity);
		}
		clientRequest.end();

	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.node.chain"></a>[function <span class="apidocSignatureSpan">rest.node.</span>chain ()](#apidoc.element.rest.node.chain)
- description and source-code
```javascript
function chain() {
		if (typeof console !== 'undefined') {
			console.log('rest.js: client.chain() is deprecated, use client.wrap() instead');
		}

		return impl.wrap.apply(this, arguments);
	}
```
- example usage
```shell
...
1.1.1
- support for IE 11, Safari 7 and iOS 7 (no code changes required, now actively testing)
- Node specific configuration options via request.mixin. Particularly useful for https clients. Thanks @wwwdata
- basic support for Browserify. Note: Browserify is not yet a tested environment

1.1.0
- bump when.js version to ~3, 2.x is no longer supported
- perfer 'client.wrap()' to 'client.chain()', 'chain' is now deprecated
- add HTTP specific methods to the promises returned from clients: .entity(), .status(), .headers(), .header(name)
- mime converters may return a promise. Thanks @phillipj
- removed 'rest/util/beget' favor Object.create

1.0.3
- add moduleType for bower (node and amd). Thanks @briancavalier
- doc polish. Thanks @gogamoga
...
```

#### <a name="apidoc.element.rest.node.wrap"></a>[function <span class="apidocSignatureSpan">rest.node.</span>wrap (interceptor, config)](#apidoc.element.rest.node.wrap)
- description and source-code
```javascript
function wrap(interceptor, config) {
		return interceptor(impl, config);
	}
```
- example usage
```shell
...

'''javascript
var rest, mime, client;

rest = require('rest'),
mime = require('rest/interceptor/mime');

client = rest.wrap(mime);
client({ path: '/data.json' }).then(function(response) {
    console.log('response: ', response);
});
'''

Before an interceptor can be used, it needs to be configured.  In this case, we will accept the default configuration, and obtain
 a client.  Now when we see the response, the entity will be a JS object instead of a String.
...
```



# <a name="apidoc.module.rest.pubsub"></a>[module rest.pubsub](#apidoc.module.rest.pubsub)

#### <a name="apidoc.element.rest.pubsub.publish"></a>[function <span class="apidocSignatureSpan">rest.pubsub.</span>publish (topic)](#apidoc.element.rest.pubsub.publish)
- description and source-code
```javascript
function publish(topic) {
	if (!topics[topic]) { return; }
	topics[topic].apply({}, Array.prototype.slice.call(arguments, 1));
	// auto cleanup
	delete topics[topic];
}
```
- example usage
```shell
...
	m = regex.exec(queryString);
	do {
		params[decodeURIComponent(m[1])] = decodeURIComponent(m[2]);
		m = regex.exec(queryString);
	} while (m);

	/*jshint camelcase:false */
	pubsub.publish(params.state, params.token_type + ' ' + params.access_token);
}

function defaultWindowStrategy(url) {
	var w = window.open(url, '_blank', 'width=500,height=400');
	return function () {
		w.close();
	};
...
```

#### <a name="apidoc.element.rest.pubsub.subscribe"></a>[function <span class="apidocSignatureSpan">rest.pubsub.</span>subscribe (topic, callback)](#apidoc.element.rest.pubsub.subscribe)
- description and source-code
```javascript
function subscribe(topic, callback) {
	topics[topic] = callback;
}
```
- example usage
```shell
...
			'client_id': config.clientId,
			'scope': config.scope,
			'state': state
		});

		dismissWindow = config.windowStrategy(url);

		pubsub.subscribe(state, function (authorization) {
			dismissWindow();
			resolve(authorization);
		});

	});
}
...
```



# <a name="apidoc.module.rest.registry"></a>[module rest.registry](#apidoc.module.rest.registry)

#### <a name="apidoc.element.rest.registry.child"></a>[function <span class="apidocSignatureSpan">rest.registry.</span>child ()](#apidoc.element.rest.registry.child)
- description and source-code
```javascript
function child() {
		return new Registry(Object.create(mimes));
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.registry.delegate"></a>[function <span class="apidocSignatureSpan">rest.registry.</span>delegate (type)](#apidoc.element.rest.registry.delegate)
- description and source-code
```javascript
function delegate(type) {
		return {
			read: function () {
				var args = arguments;
				return this.lookup(type).then(function (converter) {
					return converter.read.apply(this, args);
				}.bind(this));
			}.bind(this),
			write: function () {
				var args = arguments;
				return this.lookup(type).then(function (converter) {
					return converter.write.apply(this, args);
				}.bind(this));
			}.bind(this)
		};
	}
```
- example usage
```shell
...
// include provided serializers
registry.register('application/hal', require('./type/application/hal'));
registry.register('application/json', require('./type/application/json'));
registry.register('application/x-www-form-urlencoded', require('./type/application/x-www-form-urlencoded'));
registry.register('multipart/form-data', require('./type/multipart/form-data'));
registry.register('text/plain', require('./type/text/plain'));

registry.register('+json', registry.delegate('application/json'));

module.exports = registry;
...
```

#### <a name="apidoc.element.rest.registry.lookup"></a>[function <span class="apidocSignatureSpan">rest.registry.</span>lookup (type)](#apidoc.element.rest.registry.lookup)
- description and source-code
```javascript
function lookup(type) {
		var parsed;

		parsed = typeof type === 'string' ? mime.parse(type) : type;

		if (mimes[parsed.raw]) {
			return mimes[parsed.raw];
		}
		if (mimes[parsed.type + parsed.suffix]) {
			return mimes[parsed.type + parsed.suffix];
		}
		if (mimes[parsed.type]) {
			return mimes[parsed.type];
		}
		if (mimes[parsed.suffix]) {
			return mimes[parsed.suffix];
		}

		return Promise.reject(new Error('Unable to locate converter for mime "' + parsed.raw + '"'));
	}
```
- example usage
```shell
...

		if (!('entity' in request)) {
			return request;
		}

		headers['Content-Type'] = type.raw;

		return config.registry.lookup(type)['catch'](function () {
			// failed to resolve converter
			if (config.permissive) {
				return noopConverter;
			}
			throw 'mime-unknown';
		}).then(function (converter) {
			var client = config.client || request.originator,
...
```

#### <a name="apidoc.element.rest.registry.register"></a>[function <span class="apidocSignatureSpan">rest.registry.</span>register (type, converter)](#apidoc.element.rest.registry.register)
- description and source-code
```javascript
function register(type, converter) {
		mimes[type] = Promise.resolve(converter);
		return mimes[type];
	}
```
- example usage
```shell
...


### Custom MIME Converters: ###

'''javascript
var registry = require('rest/mime/registry');

registry.register('application/vnd.com.example', {
read: function(str) {
    var obj;
    // do string to object conversions
    return obj;
},
write: function(obj) {
    var str;
...
```



# <a name="apidoc.module.rest.responsePromise"></a>[module rest.responsePromise](#apidoc.module.rest.responsePromise)

#### <a name="apidoc.element.rest.responsePromise.responsePromise"></a>[function <span class="apidocSignatureSpan">rest.</span>responsePromise (obj, callback, errback)](#apidoc.element.rest.responsePromise.responsePromise)
- description and source-code
```javascript
function responsePromise(obj, callback, errback) {
	return make(Promise.resolve(obj).then(callback, errback));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.responsePromise.make"></a>[function <span class="apidocSignatureSpan">rest.responsePromise.</span>make (promise)](#apidoc.element.rest.responsePromise.make)
- description and source-code
```javascript
function make(promise) {
	promise.status = status;
	promise.headers = headers;
	promise.header = header;
	promise.entity = entity;
	promise.follow = follow;
	return promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.responsePromise.promise"></a>[function <span class="apidocSignatureSpan">rest.responsePromise.</span>promise (func)](#apidoc.element.rest.responsePromise.promise)
- description and source-code
```javascript
promise = function (func) {
	return make(new Promise(func));
}
```
- example usage
```shell
...
 * @param {string} [request.callback.name=<generated>] pins the name of the
 *   callback function, useful for cases where the server doesn't allow
 *   custom callback names. Generally not recommended.
 *
 * @returns {Promise<Response>}
 */
module.exports = client(function jsonp(request) {
	return responsePromise.promise(function (resolve, reject) {

		var callbackName, callbackParams, script, firstScript, response;

		request = typeof request === 'string' ? { path: request } : request || {};
		response = { request: request };

		if (request.canceled) {
...
```

#### <a name="apidoc.element.rest.responsePromise.reject"></a>[function <span class="apidocSignatureSpan">rest.responsePromise.</span>reject (val)](#apidoc.element.rest.responsePromise.reject)
- description and source-code
```javascript
reject = function (val) {
	return make(Promise.reject(val));
}
```
- example usage
```shell
...
module.exports = interceptor({
	init: function (config) {
		config.code = config.code || 400;
		return config;
	},
	response: function (response, config) {
		if (response.status && response.status.code >= config.code) {
			return Promise.reject(response);
		}
		return response;
	}
});
...
```



# <a name="apidoc.module.rest.rfc5988"></a>[module rest.rfc5988](#apidoc.module.rest.rfc5988)

#### <a name="apidoc.element.rest.rfc5988.SyntaxError"></a>[function <span class="apidocSignatureSpan">rest.rfc5988.</span>SyntaxError (expected, found, offset, line, column)](#apidoc.element.rest.rfc5988.SyntaxError)
- description and source-code
```javascript
SyntaxError = function (expected, found, offset, line, column) {
  function buildMessage(expected, found) {
    var expectedHumanized, foundHumanized;

    switch (expected.length) {
      case 0:
        expectedHumanized = "end of input";
        break;
      case 1:
        expectedHumanized = expected[0];
        break;
      default:
        expectedHumanized = expected.slice(0, expected.length - 1).join(", ")
          + " or "
          + expected[expected.length - 1];
    }

    foundHumanized = found ? quote(found) : "end of input";

    return "Expected " + expectedHumanized + " but " + foundHumanized + " found.";
  }

  this.name = "SyntaxError";
  this.expected = expected;
  this.found = found;
  this.message = buildMessage(expected, found);
  this.offset = offset;
  this.line = line;
  this.column = column;
}
```
- example usage
```shell
...
 * handle these states.
 */
if (result === null || pos !== input.length) {
  var offset = Math.max(pos, rightmostFailuresPos);
  var found = offset < input.length ? input.charAt(offset) : null;
  var errorPosition = computeErrorPosition();

  throw new this.SyntaxError(
    cleanupExpected(rightmostFailuresExpected),
    found,
    offset,
    errorPosition.line,
    errorPosition.column
  );
}
...
```

#### <a name="apidoc.element.rest.rfc5988.parse"></a>[function <span class="apidocSignatureSpan">rest.rfc5988.</span>parse (input, startRule)](#apidoc.element.rest.rfc5988.parse)
- description and source-code
```javascript
parse = function (input, startRule) {
  var parseFunctions = {
    "start": parse_start,
    "LinkValue": parse_LinkValue,
    "LinkParams": parse_LinkParams,
    "URIReference": parse_URIReference,
    "LinkParam": parse_LinkParam,
    "LinkParamName": parse_LinkParamName,
    "LinkParamValue": parse_LinkParamValue,
    "PToken": parse_PToken,
    "PTokenChar": parse_PTokenChar,
    "OptionalSP": parse_OptionalSP,
    "QuotedString": parse_QuotedString,
    "QuotedStringInternal": parse_QuotedStringInternal,
    "Char": parse_Char,
    "UpAlpha": parse_UpAlpha,
    "LoAlpha": parse_LoAlpha,
    "Alpha": parse_Alpha,
    "Digit": parse_Digit,
    "SP": parse_SP,
    "DQ": parse_DQ,
    "QDText": parse_QDText,
    "QuotedPair": parse_QuotedPair
  };

  if (startRule !== undefined) {
    if (parseFunctions[startRule] === undefined) {
      throw new Error("Invalid rule name: " + quote(startRule) + ".");
    }
  } else {
    startRule = "start";
  }

  var pos = 0;
  var reportFailures = 0;
  var rightmostFailuresPos = 0;
  var rightmostFailuresExpected = [];

  function padLeft(input, padding, length) {
    var result = input;

    var padLength = length - input.length;
    for (var i = 0; i < padLength; i++) {
      result = padding + result;
    }

    return result;
  }

  function escape(ch) {
    var charCode = ch.charCodeAt(0);
    var escapeChar;
    var length;

    if (charCode <= 0xFF) {
      escapeChar = 'x';
      length = 2;
    } else {
      escapeChar = 'u';
      length = 4;
    }

    return '\\' + escapeChar + padLeft(charCode.toString(16).toUpperCase(), '0', length);
  }

  function matchFailed(failure) {
    if (pos < rightmostFailuresPos) {
      return;
    }

    if (pos > rightmostFailuresPos) {
      rightmostFailuresPos = pos;
      rightmostFailuresExpected = [];
    }

    rightmostFailuresExpected.push(failure);
  }

  function parse_start() {
    var result0, result1, result2, result3, result4;
    var pos0, pos1, pos2, pos3;

    pos0 = pos;
    pos1 = pos;
    result0 = [];
    pos2 = pos;
    pos3 = pos;
    result1 = parse_LinkValue();
    if (result1 !== null) {
      result2 = parse_OptionalSP();
      if (result2 !== null) {
        if (input.charCodeAt(pos) === 44) {
          result3 = ",";
          pos++;
        } else {
          result3 = null;
          if (reportFailures === 0) {
            matchFailed("\",\"");
          }
        }
        if (result3 !== null) {
          result4 = parse_OptionalSP();
          if (result4 !== null) {
            result1 = [result1, result2, result3, result4];
          } else {
            result1 = null;
            pos = pos3;
          }
        } else {
          result1 = null;
          pos = pos3;
        }
      } else {
        result1 = null;
        pos = pos3;
      }
    } else {
      result1 = null;
      pos = pos3;
    }
    if (result1 !== null) {
      result1 = (function(offset, i) {return i;})(pos2, result1[0]);
    }
    if (result1 === null) {
      pos = pos2;
    }
    while (result1 !== null) {
      result0.push(result1);
      pos2 = pos;
      pos3 = pos;
      result1 = parse_LinkValue();
      if (result1 !== null) {
        result2 = parse_OptionalSP();
        if (result2 !== null) {
          if (input.charCodeAt(pos) === 44) {
            result3 = ",";
            pos++;
          } else {
            result3 = null;
            if (reportFailures === 0) {
              matchFailed("\",\"");
            }
          }
          if (result3 !== null) {
            result4 = parse_OptionalSP();
            if (result4 !== null) {
              result1 = [result1, result2, result3, result4];
            } else {
              result1 = null;
              pos = pos3;
            }
          } else {
            result1 = null;
            pos = pos3;
          }
        } else {
          result1 = null;
          pos = pos3;
        }
      } else {
        result1 = null;
        pos = pos3;
      }
      if (result1 !== null) {
        result1 = (function(offset, i) {return i;})(pos2, result1[0]);
      } ...
```
- example usage
```shell
...
			reject(response);
			return;
		}

		url = response.url = request.path || '';
		client = url.match(httpsExp) ? https : http;

		options = mixin({}, request.mixin, parser.parse(url));

		entity = request.entity;
		request.method = request.method || (entity ? 'POST' : 'GET');
		options.method = request.method;
		headers = options.headers = {};
		Object.keys(request.headers || {}).forEach(function (name) {
			headers[normalizeHeaderName(name)] = request.headers[name];
...
```

#### <a name="apidoc.element.rest.rfc5988.toSource"></a>[function <span class="apidocSignatureSpan">rest.rfc5988.</span>toSource ()](#apidoc.element.rest.rfc5988.toSource)
- description and source-code
```javascript
toSource = function () { return this._source; }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rest.uriEncoder"></a>[module rest.uriEncoder](#apidoc.module.rest.uriEncoder)

#### <a name="apidoc.element.rest.uriEncoder.decode"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>decode (str)](#apidoc.element.rest.uriEncoder.decode)
- description and source-code
```javascript
function decode(str) {
	return decodeURIComponent(str);
}
```
- example usage
```shell
...
		}
		if (prefixRE.test(variable)) {
			var prefix = prefixRE.exec(variable);
			variable = prefix[1];
			opts.maxLength = parseInt(prefix[2]);
		}

		variable = uriEncoder.decode(variable);
		value = params[variable];

		if (value === void 0 || value === null) {
			return result;
		}
		if (Array.isArray(value)) {
			result = value.reduce(function (result, value) {
...
```

#### <a name="apidoc.element.rest.uriEncoder.encode"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encode (str)](#apidoc.element.rest.uriEncoder.encode)
- description and source-code
```javascript
encode = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
...
		var headers, username, password;

		headers = request.headers || (request.headers = {});
		username = request.username || config.username;
		password = request.password || config.password || '';

		if (username) {
			headers.Authorization = 'Basic ' + base64.encode(username + ':' + password);
		}

		return request;
	}
});
...
```

#### <a name="apidoc.element.rest.uriEncoder.encodeFragment"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeFragment (str)](#apidoc.element.rest.uriEncoder.encodeFragment)
- description and source-code
```javascript
encodeFragment = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodeHost"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeHost (str)](#apidoc.element.rest.uriEncoder.encodeHost)
- description and source-code
```javascript
encodeHost = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodePath"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodePath (str)](#apidoc.element.rest.uriEncoder.encodePath)
- description and source-code
```javascript
encodePath = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodePathSegment"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodePathSegment (str)](#apidoc.element.rest.uriEncoder.encodePathSegment)
- description and source-code
```javascript
encodePathSegment = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodePort"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodePort (str)](#apidoc.element.rest.uriEncoder.encodePort)
- description and source-code
```javascript
encodePort = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodeQuery"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeQuery (str)](#apidoc.element.rest.uriEncoder.encodeQuery)
- description and source-code
```javascript
encodeQuery = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodeScheme"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeScheme (str)](#apidoc.element.rest.uriEncoder.encodeScheme)
- description and source-code
```javascript
encodeScheme = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodeURL"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeURL (str)](#apidoc.element.rest.uriEncoder.encodeURL)
- description and source-code
```javascript
encodeURL = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.uriEncoder.encodeUserInfo"></a>[function <span class="apidocSignatureSpan">rest.uriEncoder.</span>encodeUserInfo (str)](#apidoc.element.rest.uriEncoder.encodeUserInfo)
- description and source-code
```javascript
encodeUserInfo = function (str) {
		return encode(str, allowed);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rest.uriTemplate"></a>[module rest.uriTemplate](#apidoc.module.rest.uriTemplate)

#### <a name="apidoc.element.rest.uriTemplate.expand"></a>[function <span class="apidocSignatureSpan">rest.uriTemplate.</span>expand (template, params)](#apidoc.element.rest.uriTemplate.expand)
- description and source-code
```javascript
function expandTemplate(template, params) {
	var start, end, uri;

	uri = '';
	end = 0;
	while (true) {
		start = template.indexOf('{', end);
		if (start === -1) {
			// no more expressions
			uri += template.slice(end);
			break;
		}
		uri += template.slice(end, start);
		end = template.indexOf('}', start) + 1;
		uri += expandExpression(template.slice(start + 1, end - 1), params);
	}

	return uri;
}
```
- example usage
```shell
...
	},
	request: function (request, config) {
		var template, params;

		template = request.path || config.template;
		params = mixin({}, request.params, config.params);

		request.path = uriTemplate.expand(template, params);
		delete request.params;

		return request;
	}
});
...
```



# <a name="apidoc.module.rest.xhr"></a>[module rest.xhr](#apidoc.module.rest.xhr)

#### <a name="apidoc.element.rest.xhr.xhr"></a>[function <span class="apidocSignatureSpan">rest.</span>xhr (request)](#apidoc.element.rest.xhr.xhr)
- description and source-code
```javascript
function xhr(request) {
	return responsePromise.promise(function (resolve, reject) {
		<span class="apidocCodeCommentSpan">/*jshint maxcomplexity:20 */
</span>
		var client, method, url, headers, entity, headerName, response, XHR;

		request = typeof request === 'string' ? { path: request } : request || {};
		response = { request: request };

		if (request.canceled) {
			response.error = 'precanceled';
			reject(response);
			return;
		}

		XHR = request.engine || XMLHttpRequest;
		if (!XHR) {
			reject({ request: request, error: 'xhr-not-available' });
			return;
		}

		entity = request.entity;
		request.method = request.method || (entity ? 'POST' : 'GET');
		method = request.method;
		url = response.url = request.path || '';

		try {
			client = response.raw = new XHR();

			// mixin extra request properties before and after opening the request as some properties require being set at different phases
 of the request
			safeMixin(client, request.mixin);
			client.open(method, url, true);
			safeMixin(client, request.mixin);

			headers = request.headers;
			for (headerName in headers) {
				/*jshint forin:false */
				if (headerName === 'Content-Type' && headers[headerName] === 'multipart/form-data') {
					// XMLHttpRequest generates its own Content-Type header with the
					// appropriate multipart boundary when sending multipart/form-data.
					continue;
				}

				client.setRequestHeader(headerName, headers[headerName]);
			}

			request.canceled = false;
			request.cancel = function cancel() {
				request.canceled = true;
				client.abort();
				reject(response);
			};

			client.onreadystatechange = function (/* e */) {
				if (request.canceled) { return; }
				if (client.readyState === (XHR.DONE || 4)) {
					response.status = {
						code: client.status,
						text: client.statusText
					};
					response.headers = parseHeaders(client.getAllResponseHeaders());
					response.entity = client.responseText;

					// #125 -- Sometimes IE8-9 uses 1223 instead of 204
					// http://stackoverflow.com/questions/10046972/msie-returns-status-code-of-1223-for-ajax-request
					if (response.status.code === 1223) {
						response.status.code = 204;
					}

					if (response.status.code > 0) {
						// check status code as readystatechange fires before error event
						resolve(response);
					}
					else {
						// give the error callback a chance to fire before resolving
						// requests for file:// URLs do not have a status code
						setTimeout(function () {
							resolve(response);
						}, 0);
					}
				}
			};

			try {
				client.onerror = function (/* e */) {
					response.error = 'loaderror';
					reject(response);
				};
			}
			catch (e) {
				// IE 6 will not support error handling
			}

			client.send(entity);
		}
		catch (e) {
			response.error = 'loaderror';
			reject(response);
		}

	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rest.xhr.chain"></a>[function <span class="apidocSignatureSpan">rest.xhr.</span>chain ()](#apidoc.element.rest.xhr.chain)
- description and source-code
```javascript
function chain() {
		if (typeof console !== 'undefined') {
			console.log('rest.js: client.chain() is deprecated, use client.wrap() instead');
		}

		return impl.wrap.apply(this, arguments);
	}
```
- example usage
```shell
...
1.1.1
- support for IE 11, Safari 7 and iOS 7 (no code changes required, now actively testing)
- Node specific configuration options via request.mixin. Particularly useful for https clients. Thanks @wwwdata
- basic support for Browserify. Note: Browserify is not yet a tested environment

1.1.0
- bump when.js version to ~3, 2.x is no longer supported
- perfer 'client.wrap()' to 'client.chain()', 'chain' is now deprecated
- add HTTP specific methods to the promises returned from clients: .entity(), .status(), .headers(), .header(name)
- mime converters may return a promise. Thanks @phillipj
- removed 'rest/util/beget' favor Object.create

1.0.3
- add moduleType for bower (node and amd). Thanks @briancavalier
- doc polish. Thanks @gogamoga
...
```

#### <a name="apidoc.element.rest.xhr.wrap"></a>[function <span class="apidocSignatureSpan">rest.xhr.</span>wrap (interceptor, config)](#apidoc.element.rest.xhr.wrap)
- description and source-code
```javascript
function wrap(interceptor, config) {
		return interceptor(impl, config);
	}
```
- example usage
```shell
...

'''javascript
var rest, mime, client;

rest = require('rest'),
mime = require('rest/interceptor/mime');

client = rest.wrap(mime);
client({ path: '/data.json' }).then(function(response) {
    console.log('response: ', response);
});
'''

Before an interceptor can be used, it needs to be configured.  In this case, we will accept the default configuration, and obtain
 a client.  Now when we see the response, the entity will be a JS object instead of a String.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
