<% set "Operation" (capitalize (get "operation")) %>
<% set "OperationLow" (lower (get "operation")) %>
<% set "Watermarktype" (capitalize (get "watermarktype")) %>
<% set "WatermarktypeLow" (lower (get "watermarktype")) %>
<% set "FileFormat" (get "fileformat") %>
<% set "FileFormatUp" (upper (get "fileformat")) %>
<% set "FileformatCap" (capitalize (get "fileformat")) %>
<% set "EnvName" (dict "products.{product}.environmentName") %>
<% set "ProdCode" (dict "products.{product}.productCode") %>
<% set "NameProduct" (dict "products.nameProduct") %>
<% set "ProdShortName" (dict "products.productShortName") %>
<% set "ProdFullName" (dict "products.{product}.productFullName") %>
<% set "ProgLang" (dict "products.{product}.programmingLanguage") %>
<% set "SrcFileExt" (dict "products.{product}.srcFileExt") %>
<% set "DevelopmentEnvironment" (dict "products.{product}.developmentEnvironment") %>
<% set "Runtime" (dict "products.{product}.runtime") %>
<% set "ProductUrl" (dict "products.{product}.productUrl") %>
<% set "PackageStoreName" (dict "products.{product}.packageStoreName") %>
<% set "PackageUrl" (dict "products.{product}.packageUrl") %>
<% set "PricesUrl" (dict "products.{product}.pricesUrl") %>
<% set "DocsUrl" (dict "products.{product}.docsUrl") %>
<% set "MoreLink" (dict "products.{product}.more_link") %>
<% set "ReleaseDownloads" (dict "products.{product}.release_downloads") %>