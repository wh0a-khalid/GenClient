﻿# Generate Client
API Client Generator

<img src="https://www.sovtech.co.uk/wp-content/uploads/sites/11/2019/07/sovtech_logo.png"/>

## Usage

### To generate a sample client library
You can build a client against the [Vumatel API](https://raw.githubusercontent.com/pablobrincat/genclient/master/src/vumatel.json) as follows:

Run `.\bin\genclient.bat` 

This script uses the default library, which is `okhttp-gson`. It will run the generator with this command:

```sh
npx @openapitools/openapi-generator-cli generate 
-i swagger.json 
-g csharp-netcore 
-o Api.Client.Sdk
-c src/config.json
```

---
title: Config Options for csharp-netcore
sidebar_label: csharp-netcore
---

These options may be applied as additional-properties (cli) or configOptions (plugins).

| Option | Description | Values | Default |
| ------ | ----------- | ------ | ------- |
|allowUnicodeIdentifiers|boolean, toggles whether unicode identifiers are allowed in names or not, default is false| |false|
|caseInsensitiveResponseHeaders|Make API response's headers case-insensitive| |false|
|disallowAdditionalPropertiesIfNotPresent|Specify the behavior when the 'additionalProperties' keyword is not present in the OAS document. If false: the 'additionalProperties' implementation is compliant with the OAS and JSON schema specifications. If true: when the 'additionalProperties' keyword is not present in a schema, the value of 'additionalProperties' is set to false, i.e. no additional properties are allowed. Note: this mode is not compliant with the JSON schema specification. This is the original openapi-generator behavior.This setting is currently ignored for OAS 2.0 documents:  1) When the 'additionalProperties' keyword is not present in a 2.0 schema, additional properties are NOT allowed.  2) Boolean values of the 'additionalProperties' keyword are ignored. It's as if additional properties are NOT allowed.Note: the root cause are issues #1369 and #1371, which must be resolved in the swagger-parser project.|<dl><dt>**false**</dt><dd>The 'additionalProperties' implementation is compliant with the OAS and JSON schema specifications.</dd><dt>**true**</dt><dd>when the 'additionalProperties' keyword is not present in a schema, the value of 'additionalProperties' is automatically set to false, i.e. no additional properties are allowed. Note: this mode is not compliant with the JSON schema specification. This is the original openapi-generator behavior.</dd></dl>|true|
|hideGenerationTimestamp|Hides the generation timestamp when files are generated.| |true|
|interfacePrefix|Prefix interfaces with a community standard or widely accepted prefix.| |I|
|licenseId|The identifier of the license| |null|
|modelPropertyNaming|Naming convention for the property: 'camelCase', 'PascalCase', 'snake_case' and 'original', which keeps the original name| |PascalCase|
|netCoreProjectFile|Use the new format (.NET Core) for .NET project files (.csproj).| |false|
|nonPublicApi|Generates code with reduced access modifiers; allows embedding elsewhere without exposing non-public API calls to consumers.| |false|
|optionalAssemblyInfo|Generate AssemblyInfo.cs.| |true|
|optionalEmitDefaultValues|Set DataMember's EmitDefaultValue.| |false|
|optionalMethodArgument|C# Optional method argument, e.g. void square(int x=10) (.net 4.0+ only).| |true|
|optionalProjectFile|Generate {PackageName}.csproj.| |true|
|packageGuid|The GUID that will be associated with the C# project| |null|
|packageName|C# package name (convention: Title.Case).| |Org.OpenAPITools|
|packageTags|Tags to identify the package| |null|
|packageVersion|C# package version.| |1.0.0|
|releaseNote|Release note, default to 'Minor update'.| |Minor update|
|returnICollection|Return ICollection&lt;T&gt; instead of the concrete type.| |false|
|sortParamsByRequiredFlag|Sort method arguments to place required parameters before optional parameters.| |true|
|sourceFolder|source folder for generated code| |src|
|targetFramework|The target .NET framework version.|<dl><dt>**netstandard1.3**</dt><dd>.NET Standard 1.3 compatible</dd><dt>**netstandard1.4**</dt><dd>.NET Standard 1.4 compatible</dd><dt>**netstandard1.5**</dt><dd>.NET Standard 1.5 compatible</dd><dt>**netstandard1.6**</dt><dd>.NET Standard 1.6 compatible</dd><dt>**netstandard2.0**</dt><dd>.NET Standard 2.0 compatible</dd><dt>**netstandard2.1**</dt><dd>.NET Standard 2.1 compatible</dd><dt>**netcoreapp2.0**</dt><dd>.NET Core 2.0 compatible</dd><dt>**netcoreapp2.1**</dt><dd>.NET Core 2.1 compatible</dd><dt>**netcoreapp3.0**</dt><dd>.NET Core 3.0 compatible</dd><dt>**netcoreapp3.1**</dt><dd>.NET Core 3.1 compatible</dd><dt>**net47**</dt><dd>.NET Framework 4.7 compatible</dd></dl>|netstandard2.0|
|useCollection|Deserialize array types to Collection&lt;T&gt; instead of List&lt;T&gt;.| |false|
|useDateTimeOffset|Use DateTimeOffset to model date-time properties| |false|
|useOneOfDiscriminatorLookup|Use the discriminator's mapping in oneOf to speed up the model lookup. IMPORTANT: Validation (e.g. one and onlye one match in oneOf's schemas) will be skipped.| |false|
|validatable|Generates self-validatable models.| |true|

## IMPORT MAPPING

| Type/Alias | Imports |
| ---------- | ------- |


## INSTANTIATION TYPES

| Type/Alias | Instantiated By |
| ---------- | --------------- |
|array|List|
|list|List|
|map|Dictionary|


## LANGUAGE PRIMITIVES

<ul class="column-ul">
<li>Boolean</li>
<li>Collection</li>
<li>DateTime</li>
<li>DateTime?</li>
<li>DateTimeOffset</li>
<li>DateTimeOffset?</li>
<li>Decimal</li>
<li>Dictionary</li>
<li>Double</li>
<li>Float</li>
<li>Guid</li>
<li>Guid?</li>
<li>ICollection</li>
<li>Int32</li>
<li>Int64</li>
<li>List</li>
<li>Object</li>
<li>String</li>
<li>System.IO.Stream</li>
<li>bool</li>
<li>bool?</li>
<li>byte[]</li>
<li>decimal</li>
<li>decimal?</li>
<li>double</li>
<li>double?</li>
<li>float</li>
<li>float?</li>
<li>int</li>
<li>int?</li>
<li>long</li>
<li>long?</li>
<li>string</li>
</ul>

## RESERVED WORDS

<ul class="column-ul">
<li>Client</li>
<li>abstract</li>
<li>as</li>
<li>base</li>
<li>bool</li>
<li>break</li>
<li>byte</li>
<li>case</li>
<li>catch</li>
<li>char</li>
<li>checked</li>
<li>class</li>
<li>client</li>
<li>const</li>
<li>continue</li>
<li>decimal</li>
<li>default</li>
<li>delegate</li>
<li>do</li>
<li>double</li>
<li>else</li>
<li>enum</li>
<li>event</li>
<li>explicit</li>
<li>extern</li>
<li>false</li>
<li>finally</li>
<li>fixed</li>
<li>float</li>
<li>for</li>
<li>foreach</li>
<li>goto</li>
<li>if</li>
<li>implicit</li>
<li>in</li>
<li>int</li>
<li>interface</li>
<li>internal</li>
<li>is</li>
<li>localVarFileParams</li>
<li>localVarFormParams</li>
<li>localVarHeaderParams</li>
<li>localVarHttpContentType</li>
<li>localVarHttpContentTypes</li>
<li>localVarHttpHeaderAccept</li>
<li>localVarHttpHeaderAccepts</li>
<li>localVarPath</li>
<li>localVarPathParams</li>
<li>localVarPostBody</li>
<li>localVarQueryParams</li>
<li>localVarResponse</li>
<li>localVarStatusCode</li>
<li>lock</li>
<li>long</li>
<li>namespace</li>
<li>new</li>
<li>null</li>
<li>object</li>
<li>operator</li>
<li>out</li>
<li>override</li>
<li>parameter</li>
<li>params</li>
<li>private</li>
<li>protected</li>
<li>public</li>
<li>readonly</li>
<li>ref</li>
<li>return</li>
<li>sbyte</li>
<li>sealed</li>
<li>short</li>
<li>sizeof</li>
<li>stackalloc</li>
<li>static</li>
<li>string</li>
<li>struct</li>
<li>switch</li>
<li>this</li>
<li>throw</li>
<li>true</li>
<li>try</li>
<li>typeof</li>
<li>uint</li>
<li>ulong</li>
<li>unchecked</li>
<li>unsafe</li>
<li>ushort</li>
<li>using</li>
<li>virtual</li>
<li>void</li>
<li>volatile</li>
<li>while</li>
</ul>

## FEATURE SET


### Client Modification Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|BasePath|✓|ToolingExtension
|Authorizations|✗|ToolingExtension
|UserAgent|✓|ToolingExtension
|MockServer|✗|ToolingExtension

### Data Type Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|Custom|✗|OAS2,OAS3
|Int32|✓|OAS2,OAS3
|Int64|✓|OAS2,OAS3
|Float|✓|OAS2,OAS3
|Double|✓|OAS2,OAS3
|Decimal|✓|ToolingExtension
|String|✓|OAS2,OAS3
|Byte|✓|OAS2,OAS3
|Binary|✓|OAS2,OAS3
|Boolean|✓|OAS2,OAS3
|Date|✓|OAS2,OAS3
|DateTime|✓|OAS2,OAS3
|Password|✓|OAS2,OAS3
|File|✓|OAS2
|Array|✓|OAS2,OAS3
|Maps|✓|ToolingExtension
|CollectionFormat|✓|OAS2
|CollectionFormatMulti|✓|OAS2
|Enum|✓|OAS2,OAS3
|ArrayOfEnum|✓|ToolingExtension
|ArrayOfModel|✓|ToolingExtension
|ArrayOfCollectionOfPrimitives|✓|ToolingExtension
|ArrayOfCollectionOfModel|✓|ToolingExtension
|ArrayOfCollectionOfEnum|✓|ToolingExtension
|MapOfEnum|✓|ToolingExtension
|MapOfModel|✓|ToolingExtension
|MapOfCollectionOfPrimitives|✓|ToolingExtension
|MapOfCollectionOfModel|✓|ToolingExtension
|MapOfCollectionOfEnum|✓|ToolingExtension

### Documentation Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|Readme|✓|ToolingExtension
|Model|✓|ToolingExtension
|Api|✓|ToolingExtension

### Global Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|Host|✓|OAS2,OAS3
|BasePath|✓|OAS2,OAS3
|Info|✓|OAS2,OAS3
|Schemes|✗|OAS2,OAS3
|PartialSchemes|✓|OAS2,OAS3
|Consumes|✓|OAS2
|Produces|✓|OAS2
|ExternalDocumentation|✓|OAS2,OAS3
|Examples|✓|OAS2,OAS3
|XMLStructureDefinitions|✗|OAS2,OAS3
|MultiServer|✗|OAS3
|ParameterizedServer|✗|OAS3
|ParameterStyling|✗|OAS3
|Callbacks|✗|OAS3
|LinkObjects|✗|OAS3

### Parameter Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|Path|✓|OAS2,OAS3
|Query|✓|OAS2,OAS3
|Header|✓|OAS2,OAS3
|Body|✓|OAS2
|FormUnencoded|✓|OAS2
|FormMultipart|✓|OAS2
|Cookie|✓|OAS3

### Schema Support Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|Simple|✓|OAS2,OAS3
|Composite|✓|OAS2,OAS3
|Polymorphism|✓|OAS2,OAS3
|Union|✗|OAS3

### Security Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|BasicAuth|✓|OAS2,OAS3
|ApiKey|✓|OAS2,OAS3
|OpenIDConnect|✗|OAS3
|BearerToken|✗|OAS3
|OAuth2_Implicit|✓|OAS2,OAS3
|OAuth2_Password|✗|OAS2,OAS3
|OAuth2_ClientCredentials|✗|OAS2,OAS3
|OAuth2_AuthorizationCode|✗|OAS2,OAS3

### Wire Format Feature
| Name | Supported | Defined By |
| ---- | --------- | ---------- |
|JSON|✓|OAS2,OAS3
|XML|✓|OAS2,OAS3
|PROTOBUF|✗|ToolingExtension
|Custom|✗|OAS2,OAS3

You can also get the options with the `help generate` command (below only shows partial results):

```
NAME
        openapi-generator-cli generate - Generate code with the specified
        generator.

SYNOPSIS
        openapi-generator-cli generate
                [(-a <authorization> | --auth <authorization>)]
                [--api-name-suffix <api name suffix>] [--api-package <api package>]
                [--artifact-id <artifact id>] [--artifact-version <artifact version>]
                [(-c <configuration file> | --config <configuration file>)] [--dry-run]
                [(-e <templating engine> | --engine <templating engine>)]
                [--enable-post-process-file]
                [(-g <generator name> | --generator-name <generator name>)]
                [--generate-alias-as-model] [--git-host <git host>]
                [--git-repo-id <git repo id>] [--git-user-id <git user id>]
                [--global-property <global properties>...] [--group-id <group id>]
                [--http-user-agent <http user agent>]
                [(-i <spec file> | --input-spec <spec file>)]
                [--ignore-file-override <ignore file override location>]
                [--import-mappings <import mappings>...]
                [--instantiation-types <instantiation types>...]
                [--invoker-package <invoker package>]
                [--language-specific-primitives <language specific primitives>...]
                [--legacy-discriminator-behavior] [--library <library>]
                [--log-to-stderr] [--minimal-update]
                [--model-name-prefix <model name prefix>]
                [--model-name-suffix <model name suffix>]
                [--model-package <model package>]
                [(-o <output directory> | --output <output directory>)] [(-p <additional properties> | --additional-properties <additional properties>)...]
                [--package-name <package name>] [--release-note <release note>]
                [--remove-operation-id-prefix]
                [--reserved-words-mappings <reserved word mappings>...]
                [(-s | --skip-overwrite)] [--server-variables <server variables>...]
                [--skip-validate-spec] [--strict-spec <true/false strict behavior>]
                [(-t <template directory> | --template-dir <template directory>)]
                [--type-mappings <type mappings>...] [(-v | --verbose)]

OPTIONS
        -a <authorization>, --auth <authorization>
            adds authorization headers when fetching the OpenAPI definitions
            remotely. Pass in a URL-encoded string of name:header with a comma
            separating multiple values

...... (results omitted)

        -v, --verbose
            verbose mode

```

You can then compile and run the client, as well as unit tests against it.
