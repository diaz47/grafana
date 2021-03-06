+++
# -----------------------------------------------------------------------
# Do not edit this file. It is automatically generated by API Documenter.
# -----------------------------------------------------------------------
title = "@grafana/data"
keywords = ["grafana","documentation","sdk","@grafana/data"]
type = "docs"
+++

## @grafana/data package

A library containing most of the core functionality and data types used in Grafana.

## Classes

|  Class | Description |
|  --- | --- |
|  [AppendedVectors](./appendedvectors/) | This may be more trouble than it is worth. This trades some computation time for RAM -- rather than allocate a new array the size of all previous arrays, this just points the correct index to their original array values |
|  [AppPlugin](./appplugin/) |  |
|  [ArrayVector](./arrayvector/) |  |
|  [BinaryOperationVector](./binaryoperationvector/) |  |
|  [CircularDataFrame](./circulardataframe/) | This dataframe can have values constantly added, and will never exceed the given capacity |
|  [CircularVector](./circularvector/) | Circular vector uses a single buffer to capture a stream of values overwriting the oldest value on add.<!-- -->This supports addting to the 'head' or 'tail' and will grow the buffer to match a configured capacity. |
|  [ConstantVector](./constantvector/) |  |
|  [CSVReader](./csvreader/) |  |
|  [DataFrameView](./dataframeview/) | <b><i>(BETA)</i></b> This abstraction will present the contents of a DataFrame as if it were a well typed javascript object Vector. |
|  [DataSourceApi](./datasourceapi/) | The main data source abstraction interface, represents an instance of a data source<!-- -->Although this is a class, datasource implementations do not \*yet\* need to extend it. As such, we can not yet add functions with default implementations. |
|  [DataSourcePlugin](./datasourceplugin/) |  |
|  [FieldCache](./fieldcache/) |  |
|  [FieldConfigEditorBuilder](./fieldconfigeditorbuilder/) | Fluent API for declarative creation of field config option editors |
|  [FieldConfigOptionsRegistry](./fieldconfigoptionsregistry/) |  |
|  [GrafanaPlugin](./grafanaplugin/) |  |
|  [LanguageProvider](./languageprovider/) |  |
|  [MutableDataFrame](./mutabledataframe/) |  |
|  [PanelOptionsEditorBuilder](./paneloptionseditorbuilder/) | Fluent API for declarative creation of panel options |
|  [PanelPlugin](./panelplugin/) |  |
|  [Registry](./registry/) |  |
|  [SortedVector](./sortedvector/) | Values are returned in the order defined by the input parameter |

## Enumerations

|  Enumeration | Description |
|  --- | --- |
|  [BinaryOperationID](./binaryoperationid/) |  |
|  [ColorScheme](./colorscheme/) |  |
|  [CoreApp](./coreapp/) |  |
|  [CSVHeaderStyle](./csvheaderstyle/) |  |
|  [DataSourceStatus](./datasourcestatus/) |  |
|  [DataTransformerID](./datatransformerid/) |  |
|  [ExploreMode](./exploremode/) |  |
|  [FieldColorMode](./fieldcolormode/) |  |
|  [FieldConfigProperty](./fieldconfigproperty/) |  |
|  [FieldMatcherID](./fieldmatcherid/) |  |
|  [FieldType](./fieldtype/) |  |
|  [FrameMatcherID](./framematcherid/) | Field name matchers |
|  [GrafanaThemeType](./grafanathemetype/) |  |
|  [LoadingState](./loadingstate/) | Represent panel data loading state. |
|  [LogLevel](./loglevel/) | Mapping of log level abbreviation to canonical log level. Supported levels are reduce to limit color variation. |
|  [LogsDedupDescription](./logsdedupdescription/) |  |
|  [LogsDedupStrategy](./logsdedupstrategy/) |  |
|  [LogsMetaKind](./logsmetakind/) |  |
|  [MappingType](./mappingtype/) |  |
|  [MatcherID](./matcherid/) |  |
|  [NullValueMode](./nullvaluemode/) |  |
|  [OrgRole](./orgrole/) |  |
|  [PluginIncludeType](./pluginincludetype/) |  |
|  [PluginSignatureStatus](./pluginsignaturestatus/) |  |
|  [PluginState](./pluginstate/) |  |
|  [PluginType](./plugintype/) |  |
|  [ReducerID](./reducerid/) |  |
|  [ThresholdsMode](./thresholdsmode/) | Display mode |
|  [VariableOrigin](./variableorigin/) |  |
|  [VariableSuggestionsScope](./variablesuggestionsscope/) |  |
|  [VizOrientation](./vizorientation/) |  |

## Functions

|  Function | Description |
|  --- | --- |
|  [addLogLevelToSeries(series, lineIndex)](./addlogleveltoseries/) |  |
|  [applyFieldOverrides(options)](./applyfieldoverrides/) | Return a copy of the DataFrame with all rules applied |
|  [arrowTableToDataFrame(table)](./arrowtabletodataframe/) |  |
|  [base64StringToArrowTable(text)](./base64stringtoarrowtable/) |  |
|  [calculateFieldStats(rows, extractor)](./calculatefieldstats/) |  |
|  [calculateLogsLabelStats(rows, label)](./calculatelogslabelstats/) |  |
|  [calculateStats(values)](./calculatestats/) |  |
|  [doStandardCalcs(field, ignoreNulls, nullAsZero)](./dostandardcalcs/) |  |
|  [eventFactory(name)](./eventfactory/) |  |
|  [findCommonLabels(labelsSets)](./findcommonlabels/) | Returns a map labels that are common to the given label sets. |
|  [findHighlightChunksInText({ searchWords, textToHighlight, })](./findhighlightchunksintext/) | Adapt findMatchesInText for react-highlight-words findChunks handler. See https://github.com/bvaughn/react-highlight-words\#props |
|  [findMatchesInText(haystack, needle)](./findmatchesintext/) | Returns a list of substring regexp matches. |
|  [findUniqueLabels(labels, commonLabels)](./finduniquelabels/) | Returns a map of labels that are in <code>labels</code>, but not in <code>commonLabels</code>. |
|  [formatLabels(labels, defaultValue)](./formatlabels/) | Serializes the given labels to a string. |
|  [formattedValueToString(val)](./formattedvaluetostring/) |  |
|  [getActiveThreshold(value, thresholds)](./getactivethreshold/) |  |
|  [getDataFrameRow(data, row)](./getdataframerow/) | Wrapper to get an array from each field value |
|  [getDecimalsForValue(value, decimalOverride)](./getdecimalsforvalue/) |  |
|  [getDisplayProcessor(options)](./getdisplayprocessor/) |  |
|  [getDisplayValueAlignmentFactors(values)](./getdisplayvaluealignmentfactors/) |  |
|  [getFieldDisplayName(field, frame, allFrames)](./getfielddisplayname/) |  |
|  [getFieldMatcher(config)](./getfieldmatcher/) |  |
|  [getFlotPairs({ xField, yField, nullValueMode })](./getflotpairs/) |  |
|  [getFlotPairsConstant(seriesData, range)](./getflotpairsconstant/) | Returns a constant series based on the first value from the provide series. |
|  [getFrameDisplayName(frame, index)](./getframedisplayname/) | Get an appropriate display title |
|  [getFrameMatchers(config)](./getframematchers/) |  |
|  [getLogLevel(line)](./getloglevel/) | Returns the log level of a log line. Parse the line for level words. If no level is found, it returns <code>LogLevel.unknown</code>.<!-- -->Example: <code>getLogLevel('WARN 1999-12-31 this is great') // LogLevel.warn</code> |
|  [getLogLevelFromKey(key)](./getloglevelfromkey/) |  |
|  [getParser(line)](./getparser/) |  |
|  [getScaleCalculator(field, theme)](./getscalecalculator/) |  |
|  [getValueFormat(id)](./getvalueformat/) |  |
|  [getValueFormats()](./getvalueformats/) |  |
|  [getValueFormatterIndex()](./getvalueformatterindex/) |  |
|  [grafanaDataFrameToArrowTable(data)](./grafanadataframetoarrowtable/) |  |
|  [guessFieldTypeForField(field)](./guessfieldtypeforfield/) | Looks at the data to guess the column type. This ignores any existing setting |
|  [guessFieldTypeFromNameAndValue(name, v)](./guessfieldtypefromnameandvalue/) | Given a name and value, this will pick a reasonable field type |
|  [guessFieldTypeFromValue(v)](./guessfieldtypefromvalue/) | Given a value this will guess the best column type<!-- -->TODO: better Date/Time support! Look for standard date strings? |
|  [hasLinks(field)](./haslinks/) |  |
|  [locale(value, decimals)](./locale/) |  |
|  [parseFlags(text)](./parseflags/) | Converts any mode modifiers in the text to the Javascript equivalent flag |
|  [parseLabels(labels)](./parselabels/) | Returns a map of label keys to value from an input selector string.<!-- -->Example: <code>parseLabels('{job=&quot;foo&quot;, instance=&quot;bar&quot;}) // {job: &quot;foo&quot;, instance: &quot;bar&quot;}</code> |
|  [readCSV(csv, options)](./readcsv/) |  |
|  [reduceField(options)](./reducefield/) |  |
|  [renderMarkdown(str)](./rendermarkdown/) |  |
|  [reverseDataFrame(data)](./reversedataframe/) | Returns a copy with all values reversed |
|  [scaledUnits(factor, extArray)](./scaledunits/) |  |
|  [setMarkdownOptions(optionsOverride)](./setmarkdownoptions/) |  |
|  [simpleCountUnit(symbol)](./simplecountunit/) |  |
|  [sortDataFrame(data, sortIndex, reverse)](./sortdataframe/) |  |
|  [sortThresholds(thresholds)](./sortthresholds/) | Sorts the thresholds |
|  [stringStartsAsRegEx(str)](./stringstartsasregex/) |  |
|  [stringToJsRegex(str)](./stringtojsregex/) |  |
|  [stringToMs(str)](./stringtoms/) |  |
|  [toCSV(data, config)](./tocsv/) |  |
|  [toDataFrame(data)](./todataframe/) | Inspect any object and return the results as a DataFrame |
|  [toDataFrameDTO(data)](./todataframedto/) | Returns a copy that does not include functions |
|  [toFixed(value, decimals)](./tofixed/) |  |
|  [toFixedScaled(value, decimals, scaledDecimals, additionalDecimals, ext)](./tofixedscaled/) |  |
|  [toFixedUnit(unit, asPrefix)](./tofixedunit/) |  |
|  [toFloatOrUndefined(value)](./tofloatorundefined/) |  |
|  [toIntegerOrUndefined(value)](./tointegerorundefined/) |  |
|  [toNumberString(value)](./tonumberstring/) |  |
|  [transformDataFrame(options, data)](./transformdataframe/) | Apply configured transformations to the input data |
|  [updateDatasourcePluginOption(props, key, val)](./updatedatasourcepluginoption/) |  |
|  [validateFieldConfig(config)](./validatefieldconfig/) | This checks that all options on FieldConfig make sense. It mutates any value that needs fixed. In particular this makes sure that the first threshold value is -Infinity (not valid in JSON) |
|  [vectorator(vector)](./vectorator/) | Use functional programming with your vector |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [AbsoluteTimeRange](./absolutetimerange/) |  |
|  [AnnotationEvent](./annotationevent/) |  |
|  [AnnotationQueryRequest](./annotationqueryrequest/) | Options passed to the datasource.annotationQuery method. See docs/plugins/developing/datasource.md |
|  [AppEvent](./appevent/) |  |
|  [ApplyFieldOverrideOptions](./applyfieldoverrideoptions/) |  |
|  [AppPluginMeta](./apppluginmeta/) |  |
|  [AppRootProps](./approotprops/) |  |
|  [ArrowDataFrame](./arrowdataframe/) |  |
|  [BuildInfo](./buildinfo/) | Describes the build information that will be available via the Grafana configuration. |
|  [ColorFieldConfigSettings](./colorfieldconfigsettings/) |  |
|  [Column](./column/) |  |
|  [ConfigOverrideRule](./configoverriderule/) |  |
|  [CreatePlotOverlay](./createplotoverlay/) |  |
|  [CSVConfig](./csvconfig/) |  |
|  [CSVOptions](./csvoptions/) |  |
|  [CSVParseCallbacks](./csvparsecallbacks/) |  |
|  [DataConfigSource](./dataconfigsource/) | Describes and API for exposing panel specific data configurations. |
|  [DataFrame](./dataframe/) |  |
|  [DataFrameDTO](./dataframedto/) | Like a DataFrame, but fields may be a FieldDTO |
|  [DataLink](./datalink/) | Link configuration. The values may contain variables that need to be processed before running |
|  [DataLinkClickEvent](./datalinkclickevent/) | Callback info for DataLink click events |
|  [DataLinksFieldConfigSettings](./datalinksfieldconfigsettings/) |  |
|  [DataQuery](./dataquery/) | These are the common properties available to all queries in all datasources Specific implementations will extend this interface adding the required properties for the given context |
|  [DataQueryError](./dataqueryerror/) |  |
|  [DataQueryRequest](./dataqueryrequest/) |  |
|  [DataQueryResponse](./dataqueryresponse/) |  |
|  [DataQueryTimings](./dataquerytimings/) |  |
|  [DataSourceConstructor](./datasourceconstructor/) |  |
|  [DataSourceInstanceSettings](./datasourceinstancesettings/) | Frontend settings model that is passed to Datasource constructor. This differs a bit from the model above as this data model is available to every user who has access to a data source (Viewers+). This is loaded in bootData (on page load), or from: /api/frontend/settings |
|  [DataSourceJsonData](./datasourcejsondata/) |  |
|  [DataSourcePluginComponents](./datasourceplugincomponents/) |  |
|  [DataSourcePluginMeta](./datasourcepluginmeta/) |  |
|  [DataSourcePluginOptionsEditorProps](./datasourcepluginoptionseditorprops/) |  |
|  [DataSourceSelectItem](./datasourceselectitem/) |  |
|  [DataSourceSettings](./datasourcesettings/) | Data Source instance edit model. This is returned from: /api/datasources |
|  [DataTransformerConfig](./datatransformerconfig/) |  |
|  [DataTransformerInfo](./datatransformerinfo/) |  |
|  [DateTime](./datetime/) |  |
|  [DateTimeBuiltinFormat](./datetimebuiltinformat/) |  |
|  [DateTimeDuration](./datetimeduration/) |  |
|  [DateTimeLocale](./datetimelocale/) |  |
|  [DateTimeOptions](./datetimeoptions/) | The type describing date and time options. Used for all the helper functions available to parse or format date and time values. |
|  [DateTimeOptionsWhenParsing](./datetimeoptionswhenparsing/) | The type that describes options that can be passed when parsing a date and time value. |
|  [DateTimeOptionsWithFormat](./datetimeoptionswithformat/) | The type describing the options that can be passed to the [dateTimeFormat](./data/datetimeformat.md) helper function to control how the date and time value passed to the function is formatted. |
|  [DecimalInfo](./decimalinfo/) |  |
|  [Dimension](./dimension/) |  |
|  [DisplayValue](./displayvalue/) |  |
|  [DisplayValueAlignmentFactors](./displayvaluealignmentfactors/) | These represents the display value with the longest title and text. Used to align widths and heights when displaying multiple DisplayValues |
|  [DynamicConfigValue](./dynamicconfigvalue/) |  |
|  [ExploreQueryFieldProps](./explorequeryfieldprops/) |  |
|  [ExploreStartPageProps](./explorestartpageprops/) |  |
|  [FeatureToggles](./featuretoggles/) | Describes available feature toggles in Grafana. These can be configured via the <code>conf/custom.ini</code> to enable features under development or not yet available in stable version. |
|  [Field](./field/) |  |
|  [FieldCalcs](./fieldcalcs/) |  |
|  [FieldColor](./fieldcolor/) |  |
|  [FieldConfig](./fieldconfig/) | Every property is optional<!-- -->Plugins may extend this with additional properties. Something like series overrides |
|  [FieldConfigEditorConfig](./fieldconfigeditorconfig/) |  |
|  [FieldConfigEditorProps](./fieldconfigeditorprops/) |  |
|  [FieldConfigPropertyItem](./fieldconfigpropertyitem/) |  |
|  [FieldConfigSource](./fieldconfigsource/) |  |
|  [FieldDisplay](./fielddisplay/) |  |
|  [FieldDTO](./fielddto/) | Like a field, but properties are optional and values may be a simple array |
|  [FieldMatcherInfo](./fieldmatcherinfo/) |  |
|  [FieldOverrideContext](./fieldoverridecontext/) |  |
|  [FieldOverrideEditorProps](./fieldoverrideeditorprops/) |  |
|  [FieldReducerInfo](./fieldreducerinfo/) |  |
|  [FieldState](./fieldstate/) |  |
|  [FieldWithIndex](./fieldwithindex/) |  |
|  [FlotDataPoint](./flotdatapoint/) |  |
|  [FormattedValue](./formattedvalue/) |  |
|  [FrameMatcherInfo](./framematcherinfo/) |  |
|  [GetFieldDisplayValuesOptions](./getfielddisplayvaluesoptions/) |  |
|  [GrafanaConfig](./grafanaconfig/) | Describes all the different Grafana configuration values available for an instance. |
|  [GrafanaTheme](./grafanatheme/) |  |
|  [GrafanaThemeCommons](./grafanathemecommons/) |  |
|  [GraphSeriesXY](./graphseriesxy/) | View model projection of a series |
|  [HistoryItem](./historyitem/) |  |
|  [IntervalValues](./intervalvalues/) |  |
|  [Labels](./labels/) |  |
|  [LicenseInfo](./licenseinfo/) | Describes the license information about the current running instance of Grafana. |
|  [LinkModel](./linkmodel/) | Processed Link Model. The values are ready to use |
|  [LinkModelSupplier](./linkmodelsupplier/) | Provides a way to produce links on demand<!-- -->TODO: ScopedVars in in GrafanaUI package! |
|  [LogLabelStatsModel](./loglabelstatsmodel/) |  |
|  [LogRowModel](./logrowmodel/) |  |
|  [LogSearchMatch](./logsearchmatch/) |  |
|  [LogsMetaItem](./logsmetaitem/) |  |
|  [LogsModel](./logsmodel/) |  |
|  [LogsParser](./logsparser/) |  |
|  [MatcherConfig](./matcherconfig/) |  |
|  [MetadataInspectorProps](./metadatainspectorprops/) |  |
|  [MetricFindValue](./metricfindvalue/) |  |
|  [MutableVector](./mutablevector/) | Vector with standard manipulation functions |
|  [NavModel](./navmodel/) | Interface used to describe different kinds of page titles and page navigation. Navmodels are usually generated in the backend and stored in Redux. |
|  [NavModelBreadcrumb](./navmodelbreadcrumb/) |  |
|  [NavModelItem](./navmodelitem/) |  |
|  [NumberFieldConfigSettings](./numberfieldconfigsettings/) |  |
|  [PanelData](./paneldata/) |  |
|  [PanelEditorProps](./paneleditorprops/) |  |
|  [PanelModel](./panelmodel/) |  |
|  [PanelOptionsEditorConfig](./paneloptionseditorconfig/) |  |
|  [PanelOptionsEditorItem](./paneloptionseditoritem/) |  |
|  [PanelOptionsEditorProps](./paneloptionseditorprops/) |  |
|  [PanelPluginMeta](./panelpluginmeta/) |  |
|  [PanelProps](./panelprops/) |  |
|  [PluginBuildInfo](./pluginbuildinfo/) |  |
|  [PluginConfigPage](./pluginconfigpage/) |  |
|  [PluginConfigPageProps](./pluginconfigpageprops/) |  |
|  [PluginDependencies](./plugindependencies/) |  |
|  [PluginInclude](./plugininclude/) |  |
|  [PluginMeta](./pluginmeta/) |  |
|  [PluginMetaInfo](./pluginmetainfo/) |  |
|  [QueryEditorProps](./queryeditorprops/) |  |
|  [QueryFix](./queryfix/) |  |
|  [QueryFixAction](./queryfixaction/) |  |
|  [QueryHint](./queryhint/) |  |
|  [QueryResultBase](./queryresultbase/) |  |
|  [QueryResultMeta](./queryresultmeta/) |  |
|  [QueryResultMetaNotice](./queryresultmetanotice/) | QueryResultMetaNotice is a structure that provides user notices for query result data |
|  [QueryResultMetaStat](./queryresultmetastat/) |  |
|  [RangeMap](./rangemap/) |  |
|  [RawTimeRange](./rawtimerange/) |  |
|  [ReadWriteVector](./readwritevector/) | Apache arrow vectors are Read/Write |
|  [ReduceDataOptions](./reducedataoptions/) | Options for how to turn DataFrames into an array of display values |
|  [RegexpOrNamesMatcherOptions](./regexpornamesmatcheroptions/) |  |
|  [RegistryItem](./registryitem/) |  |
|  [RegistryItemWithOptions](./registryitemwithoptions/) |  |
|  [ScaledValue](./scaledvalue/) |  |
|  [ScopedVar](./scopedvar/) |  |
|  [ScopedVars](./scopedvars/) |  |
|  [ScreenshotInfo](./screenshotinfo/) |  |
|  [SelectableValue](./selectablevalue/) | Used in select elements |
|  [SelectFieldConfigSettings](./selectfieldconfigsettings/) |  |
|  [StandardEditorProps](./standardeditorprops/) |  |
|  [StandardEditorsRegistryItem](./standardeditorsregistryitem/) |  |
|  [StringFieldConfigSettings](./stringfieldconfigsettings/) |  |
|  [TableData](./tabledata/) |  |
|  [TextMatch](./textmatch/) |  |
|  [Threshold](./threshold/) |  |
|  [ThresholdsConfig](./thresholdsconfig/) | Config that is passed to the ThresholdsEditor |
|  [ThresholdsFieldConfigSettings](./thresholdsfieldconfigsettings/) |  |
|  [TimeOption](./timeoption/) |  |
|  [TimeOptions](./timeoptions/) |  |
|  [TimeRange](./timerange/) |  |
|  [TimeSeries](./timeseries/) |  |
|  [TransformerRegistyItem](./transformerregistyitem/) |  |
|  [TransformerUIProps](./transformeruiprops/) |  |
|  [UnitFieldConfigSettings](./unitfieldconfigsettings/) |  |
|  [UserOrgDTO](./userorgdto/) |  |
|  [ValueFormat](./valueformat/) |  |
|  [ValueFormatCategory](./valueformatcategory/) |  |
|  [ValueLinkConfig](./valuelinkconfig/) |  |
|  [ValueMap](./valuemap/) |  |
|  [ValueMappingFieldConfigSettings](./valuemappingfieldconfigsettings/) |  |
|  [VariableModel](./variablemodel/) |  |
|  [VariableSuggestion](./variablesuggestion/) |  |
|  [Vector](./vector/) |  |
|  [YAxis](./yaxis/) |  |

## Namespaces

|  Namespace | Description |
|  --- | --- |
|  [AppEvents](./appevents/) |  |
|  [dateMath](./datemath/) |  |
|  [PanelEvents](./panelevents/) |  |
|  [rangeUtil](./rangeutil/) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [binaryOperators](./binaryoperators/) |  |
|  [booleanOverrideProcessor](./booleanoverrideprocessor/) |  |
|  [createDimension](./createdimension/) |  |
|  [DataLinkBuiltInVars](./datalinkbuiltinvars/) |  |
|  [dataLinksOverrideProcessor](./datalinksoverrideprocessor/) |  |
|  [dateTime](./datetime/) |  |
|  [dateTimeAsMoment](./datetimeasmoment/) |  |
|  [dateTimeFormat](./datetimeformat/) | Helper function to format date and time according to the specified options. If no options are supplied, then default values are used. For more details, see [DateTimeOptionsWithFormat](./data/datetimeoptionswithformat.md)<!-- -->. |
|  [dateTimeFormatISO](./datetimeformatiso/) | Helper function to format date and time according to the standard ISO format e.g. 2013-02-04T22:44:30.652Z. If no options are supplied, then default values are used. For more details, see [DateTimeOptionsWithFormat](./data/datetimeoptionswithformat.md)<!-- -->. |
|  [dateTimeFormatTimeAgo](./datetimeformattimeago/) | Helper function to return elapsed time since passed date. The returned value will be formatted in a human readable format e.g. 4 years ago. If no options are supplied, then default values are used. For more details, see [DateTimeOptions](./data/datetimeoptions.md)<!-- -->. |
|  [dateTimeFormatWithAbbrevation](./datetimeformatwithabbrevation/) | Helper function to format date and time according to the Grafana default formatting, but it also appends the time zone abbreviation at the end e.g. 2020-05-20 13:37:00 CET. If no options are supplied, then default values are used. For more details please see [DateTimeOptions](./data/datetimeoptions.md)<!-- -->. |
|  [dateTimeForTimeZone](./datetimefortimezone/) |  |
|  [dateTimeParse](./datetimeparse/) | Helper function to parse a number, text or Date to a DateTime value. If a timeZone is supplied the incoming value is parsed with that timeZone as a base. The only exception to this is if the passed value is in a UTC-based format. Then it will use UTC as the base. Examples on UTC-based values are Unix epoch and ISO formatted strings.<!-- -->It can also parse the Grafana quick date and time format, e.g. now-6h will be parsed as Date.now() - 6 hours and returned as a valid DateTime value.<!-- -->If no options are supplied, then default values are used. For more details please see [DateTimeOptions](./data/datetimeoptions.md)<!-- -->. |
|  [DEFAULT\_DATE\_TIME\_FORMAT](./default_date_time_format/) |  |
|  [DEFAULT\_FIELD\_DISPLAY\_VALUES\_LIMIT](./default_field_display_values_limit/) |  |
|  [DefaultTimeRange](./defaulttimerange/) |  |
|  [DefaultTimeZone](./defaulttimezone/) |  |
|  [deprecationWarning](./deprecationwarning/) |  |
|  [escapeStringForRegex](./escapestringforregex/) |  |
|  [fieldMatchers](./fieldmatchers/) |  |
|  [fieldReducers](./fieldreducers/) |  |
|  [frameMatchers](./framematchers/) |  |
|  [getAllValuesFromDimension](./getallvaluesfromdimension/) |  |
|  [getColorByName](./getcolorbyname/) |  |
|  [getColorDefinition](./getcolordefinition/) |  |
|  [getColorDefinitionByName](./getcolordefinitionbyname/) |  |
|  [getColorForTheme](./getcolorfortheme/) |  |
|  [getColorFromHexRgbOrName](./getcolorfromhexrgborname/) |  |
|  [getColorName](./getcolorname/) |  |
|  [getColumnFromDimension](./getcolumnfromdimension/) |  |
|  [getColumnsFromDimension](./getcolumnsfromdimension/) |  |
|  [getDimensionByName](./getdimensionbyname/) |  |
|  [getFieldDisplayValues](./getfielddisplayvalues/) |  |
|  [getLocaleData](./getlocaledata/) |  |
|  [getMappedValue](./getmappedvalue/) |  |
|  [getNamedColorPalette](./getnamedcolorpalette/) |  |
|  [getSeriesTimeStep](./getseriestimestep/) | Returns minimal time step from series time field |
|  [getTimeField](./gettimefield/) |  |
|  [getTimeZoneGroups](./gettimezonegroups/) |  |
|  [getValueFromDimension](./getvaluefromdimension/) |  |
|  [guessFieldTypes](./guessfieldtypes/) |  |
|  [hasMsResolution](./hasmsresolution/) | Checks if series time field has ms resolution |
|  [identityOverrideProcessor](./identityoverrideprocessor/) |  |
|  [isDataFrame](./isdataframe/) |  |
|  [isDateTime](./isdatetime/) |  |
|  [ISO\_8601](./iso_8601/) |  |
|  [isTableData](./istabledata/) |  |
|  [locationUtil](./locationutil/) |  |
|  [LogsParsers](./logsparsers/) |  |
|  [MISSING\_VALUE](./missing_value/) |  |
|  [MS\_DATE\_TIME\_FORMAT](./ms_date_time_format/) |  |
|  [numberOverrideProcessor](./numberoverrideprocessor/) |  |
|  [objRemoveUndefined](./objremoveundefined/) |  |
|  [onUpdateDatasourceJsonDataOption](./onupdatedatasourcejsondataoption/) |  |
|  [onUpdateDatasourceJsonDataOptionChecked](./onupdatedatasourcejsondataoptionchecked/) |  |
|  [onUpdateDatasourceJsonDataOptionSelect](./onupdatedatasourcejsondataoptionselect/) |  |
|  [onUpdateDatasourceOption](./onupdatedatasourceoption/) |  |
|  [onUpdateDatasourceResetOption](./onupdatedatasourceresetoption/) |  |
|  [onUpdateDatasourceSecureJsonDataOption](./onupdatedatasourcesecurejsondataoption/) |  |
|  [onUpdateDatasourceSecureJsonDataOptionSelect](./onupdatedatasourcesecurejsondataoptionselect/) |  |
|  [selectOverrideProcessor](./selectoverrideprocessor/) |  |
|  [setLocale](./setlocale/) |  |
|  [standardEditorsRegistry](./standardeditorsregistry/) |  |
|  [standardFieldConfigEditorRegistry](./standardfieldconfigeditorregistry/) |  |
|  [standardTransformers](./standardtransformers/) |  |
|  [standardTransformersRegistry](./standardtransformersregistry/) | Registry of transformation options that can be driven by stored configuration files. |
|  [stringOverrideProcessor](./stringoverrideprocessor/) |  |
|  [textUtil](./textutil/) |  |
|  [thresholdsOverrideProcessor](./thresholdsoverrideprocessor/) |  |
|  [TIME\_FORMAT](./time_format/) |  |
|  [TIME\_SERIES\_TIME\_FIELD\_NAME](./time_series_time_field_name/) |  |
|  [TIME\_SERIES\_VALUE\_FIELD\_NAME](./time_series_value_field_name/) |  |
|  [timeZoneAbbrevation](./timezoneabbrevation/) | Helper function to return only the time zone abbreviation for a given date and time value. If no options are supplied, then default values are used. For more details please see [DateTimeOptions](./data/datetimeoptions.md)<!-- -->. |
|  [timeZoneFormatUserFriendly](./timezoneformatuserfriendly/) |  |
|  [toDuration](./toduration/) |  |
|  [toLegacyResponseData](./tolegacyresponsedata/) |  |
|  [toPascalCase](./topascalcase/) |  |
|  [toUtc](./toutc/) |  |
|  [unEscapeStringFromRegex](./unescapestringfromregex/) |  |
|  [unitOverrideProcessor](./unitoverrideprocessor/) |  |
|  [updateDatasourcePluginJsonDataOption](./updatedatasourcepluginjsondataoption/) |  |
|  [updateDatasourcePluginResetOption](./updatedatasourcepluginresetoption/) |  |
|  [updateDatasourcePluginSecureJsonDataOption](./updatedatasourcepluginsecurejsondataoption/) |  |
|  [urlUtil](./urlutil/) |  |
|  [valueMappingsOverrideProcessor](./valuemappingsoverrideprocessor/) |  |
|  [VAR\_CALC](./var_calc/) |  |
|  [VAR\_CELL\_PREFIX](./var_cell_prefix/) |  |
|  [VAR\_FIELD\_LABELS](./var_field_labels/) |  |
|  [VAR\_FIELD\_NAME](./var_field_name/) |  |
|  [VAR\_SERIES\_NAME](./var_series_name/) |  |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [BinaryOperation](./binaryoperation/) |  |
|  [Color](./color/) |  |
|  [ColorDefinition](./colordefinition/) |  |
|  [DataQueryResponseData](./dataqueryresponsedata/) |  |
|  [DataSourceOptionsType](./datasourceoptionstype/) |  |
|  [DataSourceQueryType](./datasourcequerytype/) |  |
|  [DataTransformer](./datatransformer/) | Function that transform data frames (AKA transformer) |
|  [DateTimeInput](./datetimeinput/) |  |
|  [DecimalCount](./decimalcount/) |  |
|  [Dimensions](./dimensions/) |  |
|  [DisplayProcessor](./displayprocessor/) |  |
|  [DurationInput](./durationinput/) |  |
|  [DurationUnit](./durationunit/) |  |
|  [FieldMatcher](./fieldmatcher/) |  |
|  [FormatInput](./formatinput/) |  |
|  [FrameMatcher](./framematcher/) |  |
|  [GraphSeriesValue](./graphseriesvalue/) |  |
|  [InterpolateFunction](./interpolatefunction/) |  |
|  [KeyValue](./keyvalue/) |  |
|  [LegacyResponseData](./legacyresponsedata/) | Starting in v6.2 DataFrame can represent both TimeSeries and TableData |
|  [LinkTarget](./linktarget/) |  |
|  [MutableField](./mutablefield/) |  |
|  [NavIndex](./navindex/) |  |
|  [Omit\_2](./omit_2/) |  |
|  [PanelMigrationHandler](./panelmigrationhandler/) | Called when a panel is first loaded with current panel model |
|  [PanelOptionEditorsRegistry](./paneloptioneditorsregistry/) |  |
|  [PanelTypeChangedHandler](./paneltypechangedhandler/) | Called before a panel is initialized. Allows panel inspection for any updates before changing the panel type. |
|  [PreferredVisualisationType](./preferredvisualisationtype/) |  |
|  [ScaleCalculator](./scalecalculator/) |  |
|  [Subtract](./subtract/) |  |
|  [TimeFragment](./timefragment/) |  |
|  [TimeSeriesPoints](./timeseriespoints/) |  |
|  [TimeSeriesValue](./timeseriesvalue/) |  |
|  [TimeZone](./timezone/) |  |
|  [TimeZoneBrowser](./timezonebrowser/) |  |
|  [TimeZoneResolver](./timezoneresolver/) | The type to describe the time zone resolver function that will be used to access the default time zone of a user. |
|  [TimeZoneUtc](./timezoneutc/) |  |
|  [UrlQueryMap](./urlquerymap/) | Type to represent the values parsed from the query string. |
|  [UrlQueryValue](./urlqueryvalue/) | Type to represent the value of a single query variable. |
|  [ValueConverter](./valueconverter/) |  |
|  [ValueFormatter](./valueformatter/) |  |
|  [ValueMapping](./valuemapping/) |  |
|  [VariableType](./variabletype/) |  |

