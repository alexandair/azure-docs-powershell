---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: BFB9A435-C68D-4C6F-83DB-AE4B3EFB1AA0
---

# Get-AzureRmHDInsightProperties

## SYNOPSIS
Gets properties about the HDInsight service, such as available locations and capacity.

## SYNTAX

```
Get-AzureRmHDInsightProperties [-Location] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmHDInsightProperties** cmdlet gets properties specific to Azure HDInsight, such as the list of available locations, HDInsight cluster versions, and available compute capacity.

## EXAMPLES

### Example 1: Get the properties of an Azure HDInsight cluster
```
PS C:\>Get-AzureRmHDInsightProperties -Location "East US 2"
```

This command gets properties from an HDInsight service from location East US 2.

## PARAMETERS

### -Location
Specifies the location for which to fetch HDInsight properties.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS


