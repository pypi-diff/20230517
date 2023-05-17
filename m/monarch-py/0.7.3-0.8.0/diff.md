# Comparing `tmp/monarch_py-0.7.3.tar.gz` & `tmp/monarch_py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.7.3.tar", max compression
+gzip compressed data, was "monarch_py-0.8.0.tar", max compression
```

## Comparing `monarch_py-0.7.3.tar` & `monarch_py-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      955 2023-05-08 22:37:25.046450 monarch_py-0.7.3/pyproject.toml
--rw-r--r--   0        0        0       77 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1587 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     6581 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     8802 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7913 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    17565 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3737 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     8133 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     4052 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-05-08 22:37:25.046450 monarch_py-0.7.3/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-17 20:08:53.342423 monarch_py-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1630 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     7377 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11736 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     9463 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:08:53.342423 monarch_py-0.8.0/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20371 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4697 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9031 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     4052 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-05-17 20:08:53.346423 monarch_py-0.8.0/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.8.0/PKG-INFO
```

### Comparing `monarch_py-0.7.3/pyproject.toml` & `monarch_py-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.7.3"
+version = "0.8.0"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.7.3/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.8.0/src/monarch_py/association_type_mappings.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,30 @@
   object_label: Phenotypes
   category: ["biolink:DiseaseToPhenotypicFeatureAssociation"]
 - association_type: gene_phenotype
   subject_label: Genes
   object_label: Phenotypes
   category: ["biolink:GeneToPhenotypicFeatureAssociation"]
 - association_type: gene_interaction
-  subject_label: Genes
+  subject_label: Interactions
   object_label: Interactions
+  symmetric: true
   category: ["biolink:PairwiseGeneToGeneInteraction"]
 - association_type: gene_pathway
   subject_label: Genes
   object_label: Pathways
   category: ["biolink:GeneToPathwayAssociation"]
 - association_type: gene_expression
   subject_label: Genes
   object_label: Anatomy
   category: ["biolink:GeneToExpressionSiteAssociation"]
 - association_type: gene_orthology
   subject_label: Orthologs
   object_label: Orthologs
+  symmetric: true
   category: ["biolink:GeneToGeneHomologyAssociation"]
 - association_type: chemical_pathway
   subject_label: Chemicals
   object_label: Pathways
   category: ["biolink:ChemicalToPathwayAssociation"]
 - association_type: gene_function
   subject_label: Genes
```

### Comparing `monarch_py-0.7.3/src/monarch_py/cli.py` & `monarch_py-0.8.0/src/monarch_py/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import importlib
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from monarch_py import solr_cli, sql_cli
+from monarch_py.datamodels.model import AssociationTypeEnum
 
 app = typer.Typer()
 app.add_typer(solr_cli.solr_app, name="solr")
 app.add_typer(sql_cli.sql_app, name="sql")
 
 
 @app.callback(invoke_without_command=True)
@@ -68,15 +69,15 @@
     category: str = typer.Option(None, "--category", "-c"),
     subject: str = typer.Option(None, "--subject", "-s"),
     predicate: str = typer.Option(None, "--predicate", "-p"),
     object: str = typer.Option(None, "--object", "-o"),
     entity: str = typer.Option(None, "--entity", "-e"),
     between: str = typer.Option(None, "--between"),
     direct: bool = typer.Option(False, "--direct"),
-    association_type: str = typer.Option(None, "--label"),
+    association_type: str = typer.Option(None, "--association-type"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
@@ -211,9 +212,31 @@
 
     Returns:
         A list of association counts for the given entity containing association type, label and count
     """
     solr_cli.association_counts(**locals())
 
 
+@app.command("association-table")
+def association_table(
+    entity: str = typer.Argument(..., help="The entity to get associations for"),
+    association_type: AssociationTypeEnum = typer.Argument(
+        ..., help="The association type to get associations for"
+    ),
+    q: str = typer.Option(None, "--query", "-q"),
+    limit: int = typer.Option(5, "--limit", "-l"),
+    offset: int = typer.Option(0, "--offset"),
+    fmt: str = typer.Option(
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
+    ),
+    output: str = typer.Option(
+        None, "--output", "-o", help="The path to the output file"
+    ),
+):
+    solr_cli.association_table(**locals())
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `monarch_py-0.7.3/src/monarch_py/datamodels/model.py` & `monarch_py-0.8.0/src/monarch_py/datamodels/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,109 @@
 from __future__ import annotations
-from datetime import datetime, date
+
 from enum import Enum
-from typing import List, Dict, Optional, Any, Union, Literal
-from pydantic import BaseModel as BaseModel, Field
-from linkml_runtime.linkml_model import Decimal
+from typing import Dict, List, Optional
+
+from pydantic import BaseModel as BaseModel
+from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
+
 class WeakRefShimBaseModel(BaseModel):
-   __slots__ = '__weakref__'
-    
-class ConfiguredBaseModel(WeakRefShimBaseModel,
-                validate_assignment = True, 
-                validate_all = True, 
-                underscore_attrs_are_private = True, 
-                extra = 'forbid', 
-                arbitrary_types_allowed = True):
-    pass                    
+    __slots__ = "__weakref__"
+
+
+class ConfiguredBaseModel(
+    WeakRefShimBaseModel,
+    validate_assignment=True,
+    validate_all=True,
+    underscore_attrs_are_private=True,
+    extra="forbid",
+    arbitrary_types_allowed=True,
+):
+    pass
+
+
+class AssociationDirectionEnum(str, Enum):
+
+    incoming = "incoming"
+    outgoing = "outgoing"
 
 
 class AssociationTypeEnum(str, Enum):
-    
+
     disease_phenotype = "disease_phenotype"
     gene_phenotype = "gene_phenotype"
     gene_interaction = "gene_interaction"
     gene_pathway = "gene_pathway"
     gene_expression = "gene_expression"
     gene_orthology = "gene_orthology"
     chemical_pathway = "chemical_pathway"
     gene_function = "gene_function"
     correlated_gene = "correlated_gene"
     causal_gene = "causal_gene"
-    
-    
+
 
 class Association(ConfiguredBaseModel):
-    
+
     aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
     id: str = Field(None)
-    subject: Optional[str] = Field(None)
+    subject: str = Field(None)
     original_subject: Optional[str] = Field(None)
     subject_namespace: Optional[str] = Field(None)
     subject_category: Optional[List[str]] = Field(default_factory=list)
     subject_closure: Optional[List[str]] = Field(default_factory=list)
     subject_label: Optional[str] = Field(None)
     subject_closure_label: Optional[List[str]] = Field(default_factory=list)
-    predicate: Optional[str] = Field(None)
-    object: Optional[str] = Field(None)
+    predicate: str = Field(None)
+    object: str = Field(None)
+    original_object: Optional[str] = Field(None)
+    object_namespace: Optional[str] = Field(None)
+    object_category: Optional[List[str]] = Field(default_factory=list)
+    object_closure: Optional[List[str]] = Field(default_factory=list)
+    object_label: Optional[str] = Field(None)
+    object_closure_label: Optional[List[str]] = Field(default_factory=list)
+    primary_knowledge_source: Optional[List[str]] = Field(default_factory=list)
+    category: Optional[List[str]] = Field(default_factory=list)
+    negated: Optional[bool] = Field(None)
+    provided_by: Optional[str] = Field(None)
+    publications: Optional[List[str]] = Field(default_factory=list)
+    qualifiers: Optional[List[str]] = Field(default_factory=list)
+    frequency_qualifier: Optional[str] = Field(None)
+    has_evidence: Optional[str] = Field(None)
+    onset_qualifier: Optional[str] = Field(None)
+    sex_qualifier: Optional[str] = Field(None)
+    source: Optional[str] = Field(None)
+    stage_qualifier: Optional[str] = Field(None)
+    pathway: Optional[str] = Field(None)
+    relation: Optional[str] = Field(None)
+
+
+class DirectionalAssociation(Association):
+    """
+    An association that gives it's direction relative to a specified entity
+    """
+
+    direction: AssociationDirectionEnum = Field(
+        None,
+        description="""The directionality of the association relative to a given entity for an association_count. If the entity is the subject or in the subject closure, the direction is forwards, if it is the object or in the object closure, the direction is backwards.""",
+    )
+    aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
+    id: str = Field(None)
+    subject: str = Field(None)
+    original_subject: Optional[str] = Field(None)
+    subject_namespace: Optional[str] = Field(None)
+    subject_category: Optional[List[str]] = Field(default_factory=list)
+    subject_closure: Optional[List[str]] = Field(default_factory=list)
+    subject_label: Optional[str] = Field(None)
+    subject_closure_label: Optional[List[str]] = Field(default_factory=list)
+    predicate: str = Field(None)
+    object: str = Field(None)
     original_object: Optional[str] = Field(None)
     object_namespace: Optional[str] = Field(None)
     object_category: Optional[List[str]] = Field(default_factory=list)
     object_closure: Optional[List[str]] = Field(default_factory=list)
     object_label: Optional[str] = Field(None)
     object_closure_label: Optional[List[str]] = Field(default_factory=list)
     primary_knowledge_source: Optional[List[str]] = Field(default_factory=list)
@@ -64,156 +116,194 @@
     has_evidence: Optional[str] = Field(None)
     onset_qualifier: Optional[str] = Field(None)
     sex_qualifier: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     stage_qualifier: Optional[str] = Field(None)
     pathway: Optional[str] = Field(None)
     relation: Optional[str] = Field(None)
-    
 
 
 class Entity(ConfiguredBaseModel):
-    
+
     id: str = Field(None)
     category: Optional[List[str]] = Field(default_factory=list)
     name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
     type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
-    
 
 
 class HistoPheno(ConfiguredBaseModel):
-    
+
     id: str = Field(None)
-    items: List[HistoBin] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
-    
+    items: List[HistoBin] = Field(
+        default_factory=list,
+        description="""A collection of items, with the type to be overriden by slot_usage""",
+    )
 
 
 class Results(ConfiguredBaseModel):
-    
+
     limit: int = Field(None, description="""number of items to return in a response""")
     offset: int = Field(None, description="""offset into the total number of items""")
     total: int = Field(None, description="""total number of items matching a query""")
-    
 
 
 class AssociationResults(Results):
-    
-    items: List[Association] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+
+    items: List[Association] = Field(
+        default_factory=list,
+        description="""A collection of items, with the type to be overriden by slot_usage""",
+    )
+    limit: int = Field(None, description="""number of items to return in a response""")
+    offset: int = Field(None, description="""offset into the total number of items""")
+    total: int = Field(None, description="""total number of items matching a query""")
+
+
+class AssociationTableResults(Results):
+
+    items: List[DirectionalAssociation] = Field(
+        default_factory=list,
+        description="""A collection of items, with the type to be overriden by slot_usage""",
+    )
     limit: int = Field(None, description="""number of items to return in a response""")
     offset: int = Field(None, description="""offset into the total number of items""")
     total: int = Field(None, description="""total number of items matching a query""")
-    
 
 
 class EntityResults(Results):
-    
-    items: List[Entity] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+
+    items: List[Entity] = Field(
+        default_factory=list,
+        description="""A collection of items, with the type to be overriden by slot_usage""",
+    )
     limit: int = Field(None, description="""number of items to return in a response""")
     offset: int = Field(None, description="""offset into the total number of items""")
     total: int = Field(None, description="""total number of items matching a query""")
-    
 
 
 class SearchResult(Entity):
-    
-    highlight: Optional[str] = Field(None, description="""matching text snippet containing html tags""")
+
+    highlight: Optional[str] = Field(
+        None, description="""matching text snippet containing html tags"""
+    )
     score: Optional[float] = Field(None)
     id: str = Field(None)
     category: List[str] = Field(default_factory=list)
     name: str = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
     type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
-    
 
 
 class SearchResults(Results):
-    
-    items: List[SearchResult] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
-    facet_fields: Optional[Dict[str, FacetField]] = Field(default_factory=dict, description="""Collection of facet field responses with the field values and counts""")
-    facet_queries: Optional[Dict[str, FacetValue]] = Field(default_factory=dict, description="""Collection of facet query responses with the query string values and counts""")
+
+    items: List[SearchResult] = Field(
+        default_factory=list,
+        description="""A collection of items, with the type to be overriden by slot_usage""",
+    )
+    facet_fields: Optional[Dict[str, FacetField]] = Field(
+        default_factory=dict,
+        description="""Collection of facet field responses with the field values and counts""",
+    )
+    facet_queries: Optional[Dict[str, FacetValue]] = Field(
+        default_factory=dict,
+        description="""Collection of facet query responses with the query string values and counts""",
+    )
     limit: int = Field(None, description="""number of items to return in a response""")
     offset: int = Field(None, description="""offset into the total number of items""")
     total: int = Field(None, description="""total number of items matching a query""")
-    
 
 
 class FacetValue(ConfiguredBaseModel):
-    
+
     label: str = Field(None)
     count: Optional[int] = Field(None, description="""count of documents""")
-    
 
 
 class HistoBin(FacetValue):
-    
+
     id: str = Field(None)
     label: str = Field(None)
     count: Optional[int] = Field(None, description="""count of documents""")
-    
 
 
 class FacetField(ConfiguredBaseModel):
-    
+
     label: str = Field(None)
     facet_values: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
-    
 
 
 class AssociationTypeMapping(ConfiguredBaseModel):
     """
     A data class to hold the necessary information to produce association type counts for given  entities with appropriate directional labels
     """
+
     association_type: Optional[AssociationTypeEnum] = Field(None)
-    subject_label: Optional[str] = Field(None, description="""A label to describe the subjects of the association type as a whole for use in the UI""")
-    object_label: Optional[str] = Field(None, description="""A label to describe the objects of the association type as a whole for use in the UI""")
-    category: Optional[List[str]] = Field(default_factory=list, description="""The biolink categories to use in queries for this association type, assuming OR semantics""")
-    predicate: Optional[List[str]] = Field(default_factory=list, description="""The biolink predicate to use in queries for this association type, assuming OR semantics""")
-    
+    subject_label: Optional[str] = Field(
+        None,
+        description="""A label to describe the subjects of the association type as a whole for use in the UI""",
+    )
+    object_label: Optional[str] = Field(
+        None,
+        description="""A label to describe the objects of the association type as a whole for use in the UI""",
+    )
+    symmetric: bool = Field(
+        False,
+        description="""Whether the association type is symmetric, meaning that the subject and object labels should be interchangeable""",
+    )
+    category: Optional[List[str]] = Field(
+        default_factory=list,
+        description="""The biolink categories to use in queries for this association type, assuming OR semantics""",
+    )
+    predicate: List[str] = Field(
+        default_factory=list,
+        description="""The biolink predicate to use in queries for this association type, assuming OR semantics""",
+    )
 
 
 class AssociationCount(FacetValue):
-    
+
     association_type: Optional[AssociationTypeEnum] = Field(None)
     label: str = Field(None)
     count: Optional[int] = Field(None, description="""count of documents""")
-    
 
 
 class AssociationCountList(ConfiguredBaseModel):
     """
     Container class for a list of association counts
     """
-    items: List[AssociationCount] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
-    
 
+    items: List[AssociationCount] = Field(
+        default_factory=list,
+        description="""A collection of items, with the type to be overriden by slot_usage""",
+    )
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
 Association.update_forward_refs()
+DirectionalAssociation.update_forward_refs()
 Entity.update_forward_refs()
 HistoPheno.update_forward_refs()
 Results.update_forward_refs()
 AssociationResults.update_forward_refs()
+AssociationTableResults.update_forward_refs()
 EntityResults.update_forward_refs()
 SearchResult.update_forward_refs()
 SearchResults.update_forward_refs()
 FacetValue.update_forward_refs()
 HistoBin.update_forward_refs()
 FacetField.update_forward_refs()
 AssociationTypeMapping.update_forward_refs()
 AssociationCount.update_forward_refs()
 AssociationCountList.update_forward_refs()
-
```

### Comparing `monarch_py-0.7.3/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.8.0/src/monarch_py/datamodels/model.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,25 @@
   linkml: https://w3id.org/linkml/
   biolink: https://w3id.org/biolink/
 imports:
   - linkml:types
 default_range: string
 
 enums:
+  AssociationDirectionEnum:
+    description: >-
+      The directionality of an association as it relates to a specified entity, with edges being categorized
+      as incoming or outgoing
+    permissible_values:
+      incoming:
+        description: >-
+          An association for which a specified entity is the object or part of the object closure
+      outgoing:
+        description: >-
+          An association for which a specified entity is the subject or part of the subject closure
   AssociationTypeEnum:
     description: >-
       A grouping label for association types, which are not necessarily 1:1 with
       biolink categories or predicates
     permissible_values:
       disease_phenotype:
         description: >-
@@ -84,21 +95,34 @@
     - has_evidence
     - onset_qualifier
     - sex_qualifier
     - source
     - stage_qualifier
     - pathway
     - relation
+  DirectionalAssociation:
+    is_a: Association
+    description: >-
+      An association that gives it's direction relative to a specified entity
+    slots:
+      - direction
   AssociationResults:
     is_a: Results
     slots: 
       - items
     slot_usage:
       items:
         range: Association
+  AssociationTableResults:
+    is_a: Results
+    slots:
+      - items
+    slot_usage:
+      items:
+        range: DirectionalAssociation
   Entity:
     slots:
     - id
     - category
     - name
     - description
     - xref
@@ -172,21 +196,28 @@
     description: >-
       A data class to hold the necessary information to produce association type counts for given 
       entities with appropriate directional labels
     slots:
       - association_type
       - subject_label
       - object_label
+      - symmetric
       - category
       - predicate
     slot_usage:
       subject_label:
         description: A label to describe the subjects of the association type as a whole for use in the UI
       object_label:
         description: A label to describe the objects of the association type as a whole for use in the UI
+      symmetric:
+        description: >-
+          Whether the association type is symmetric, meaning that the subject and object labels should be
+          interchangeable
+        ifabsent: false
+        required: true
       category:
         description: The biolink categories to use in queries for this association type, assuming OR semantics
         multivalued: true
       predicate:
         description: The biolink predicate to use in queries for this association type, assuming OR semantics
         multivalued: true
   AssociationCount:
@@ -209,14 +240,21 @@
   category:
     multivalued: true
   count:
     description: count of documents
     range: integer
   description:
     range: string
+  direction:
+    description: >-
+      The directionality of the association relative to a given entity for an association_count.
+      If the entity is the subject or in the subject closure, the direction is forwards, if it is
+      the object or in the object closure, the direction is backwards.
+    range: AssociationDirectionEnum
+    required: true
   facet_fields:
     description: Collection of facet field responses with the field values and counts
     inlined: true
     multivalued: true
     range: FacetField
   facet_queries:
     description: Collection of facet query responses with the query string values and counts
@@ -318,14 +356,18 @@
     multivalued: true
   subject_label:
     range: string
   subject_namespace:
     range: string
   symbol:
     range: string
+  symmetric:
+    description: >-
+      Whether the association type is symmetric, i.e. the subject and object labels are interchangeable.
+    range: boolean
   synonym:
     multivalued: true
   total:
     description: total number of items matching a query
     range: integer
     required: true
   type:
```

### Comparing `monarch_py-0.7.3/src/monarch_py/datamodels/solr.py` & `monarch_py-0.8.0/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.8.0/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 from loguru import logger
 from pydantic import ValidationError
 
 from monarch_py.datamodels.model import (
     Association,
     AssociationCount,
+    AssociationDirectionEnum,
     AssociationResults,
+    AssociationTableResults,
     AssociationTypeEnum,
+    DirectionalAssociation,
     Entity,
     FacetField,
     FacetValue,
     HistoBin,
     HistoPheno,
     SearchResult,
     SearchResults,
@@ -139,14 +142,15 @@
         object: str = None,
         subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
         direct: bool = None,
         association_type: AssociationTypeEnum = None,
+        q: str = None,
         offset: int = 0,
         limit: int = 20,
     ) -> SolrQuery:
         """Populate a SolrQuery object with association filters"""
 
         query = SolrQuery(start=offset, rows=limit)
 
@@ -196,14 +200,19 @@
                 )
         if association_type:
             query.add_filter_query(
                 get_solr_query_fragment(
                     AssociationTypeMappings().get_mapping(association_type)
                 )
             )
+        if q:
+            # We don't yet have tokenization strategies for the association index, initially we'll limit searching to
+            # the visible fields in an association table plus their ID equivalents and use a wildcard query for substring matching
+            query.q = f"*{q}*"
+            query.query_fields = "subject subject_label predicate object object_label"
 
         return query
 
     ###############################
     # Implements: SearchInterface #
     ###############################
 
@@ -411,40 +420,99 @@
         for field_query in [subject_query, object_query]:
             for agm in AssociationTypeMappings.get_mappings():
                 association_type_query = get_solr_query_fragment(agm)
                 facet_queries.append(f"({association_type_query}) {field_query}")
         query.facet_queries = facet_queries
         solr = SolrService(base_url=self.base_url, core=core.ASSOCIATION)
         query_result = solr.query(query)
-        association_counts: List[AssociationCount] = []
+        association_count_dict: Dict[str, AssociationCount] = {}
+
         for k, v in query_result.facet_counts.facet_queries.items():
             if v > 0:
                 if k.endswith(subject_query):
                     original_query = (
                         k.replace(f" {subject_query}", "").lstrip("(").rstrip(")")
                     )
                     agm = get_association_type_mapping_by_query_string(original_query)
                     label = agm.object_label
                 elif k.endswith(object_query):
                     original_query = (
                         k.replace(f" {object_query}", "").lstrip("(").rstrip(")")
                     )
                     agm = get_association_type_mapping_by_query_string(original_query)
                     label = agm.subject_label
+                    # always use forward for symmetric association types
                 else:
                     raise ValueError(
                         f"Unexpected facet query when building association counts: {k}"
                     )
-                association_counts.append(
-                    AssociationCount(
-                        label=label, count=v, association_type=agm.association_type
+                # Symmetric associations need to be summed together, since both directions will be returned
+                # when searching for associations by type
+                if label in association_count_dict and agm.symmetric:
+                    association_count_dict[label].count += v
+                else:
+                    association_count_dict[label] = AssociationCount(
+                        label=label,
+                        count=v,
+                        association_type=agm.association_type,
                     )
-                )
+
+        association_counts: List[AssociationCount] = list(
+            association_count_dict.values()
+        )
         return association_counts
 
+    def get_association_table(
+        self,
+        entity: str,
+        association_type: AssociationTypeEnum,
+        q=None,
+        sort=None,
+        offset=0,
+        limit=5,
+    ) -> AssociationTableResults:
+        if sort:
+            raise NotImplementedError("Sorting is not yet implemented")
+        query = self._populate_association_query(
+            entity=entity,
+            association_type=association_type,
+            q=q,
+            offset=offset,
+            limit=limit,
+        )
+        solr = SolrService(base_url=self.base_url, core=core.ASSOCIATION)
+        query_result = solr.query(query)
+        total = query_result.response.num_found
+        associations: List[DirectionalAssociation] = []
+        for doc in query_result.response.docs:
+            try:
+                direction = self._get_association_direction(entity, doc)
+                association = DirectionalAssociation(**doc, direction=direction)
+                associations.append(association)
+            except ValidationError:
+                logger.error(f"Validation error for {doc}")
+                raise
+
+        results = AssociationResults(
+            items=associations, limit=limit, offset=offset, total=total
+        )
+
+        return results
+
+    def _get_association_direction(
+        self, entity: str, document: Dict
+    ) -> AssociationDirectionEnum:
+        if document["subject"] == entity or entity in document["subject_closure"]:
+            direction = AssociationDirectionEnum.outgoing
+        elif document["object"] == entity or entity in document["object_closure"]:
+            direction = AssociationDirectionEnum.incoming
+        else:
+            raise ValueError(f"Entity {entity} not found in association {document}")
+        return direction
+
     def _convert_facet_fields(self, solr_facet_fields: Dict) -> Dict[str, FacetField]:
         """
         Converts a list of raw solr facet fields from the solr response to a list of
         FacetField instances
 
         Args:
             facet_fields (Dict): A list of facet fields from the solr response
```

### Comparing `monarch_py-0.7.3/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.8.0/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.8.0/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.8.0/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.8.0/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.8.0/src/monarch_py/interfaces/search_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
-from monarch_py.datamodels.model import AssociationTypeEnum, FacetValue, SearchResults
+from monarch_py.datamodels.model import (
+    AssociationTableResults,
+    AssociationTypeEnum,
+    FacetValue,
+    SearchResults,
+)
 
 
 class SearchInterface(ABC):
     """Abstract interface for searching the Monarch KG in a Lucene way"""
 
     @abstractmethod
     def search(
@@ -88,7 +93,33 @@
         Get counts of associations for a given entity
         Args:
             entity (str): Entity to get association counts for
         Returns:
             List[FacetValue]: List of FacetValue objects representing the counts of associations for the given entity
         """
         raise NotImplementedError
+
+    def get_association_table(
+        self,
+        entity: str,
+        association_type: AssociationTypeEnum,
+        query=None,
+        sort=None,
+        offset=0,
+        limit=5,
+    ) -> AssociationTableResults:
+        """
+        Get associations for an entity matching a specified type, with optional search and sort parameters
+
+        Args:
+            entity (str): Entity to get associations for
+            association_type (AssociationTypeEnum): Association type to filter to
+            query (str): Query string to match against
+            sort (str): Sort order, defaults to None
+            offset (int): Offset of the first result to return, defaults to 0
+            limit (int): Limit the number of results to return, defaults to 20
+
+        Returns:
+            AssociationResults: Dataclass representing results of an association search.
+        """
+
+        raise NotImplementedError
```

### Comparing `monarch_py-0.7.3/src/monarch_py/service/solr_service.py` & `monarch_py-0.8.0/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/solr_cli.py` & `monarch_py-0.8.0/src/monarch_py/solr_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pystow
 import typer
 
-from monarch_py.datamodels.model import AssociationCountList
+from monarch_py.datamodels.model import AssociationCountList, AssociationTypeEnum
 from monarch_py.utils.solr_cli_utils import (
     check_solr_permissions,
     get_solr,
     solr_status,
     start_solr,
     stop_solr,
 )
@@ -258,7 +258,33 @@
     if not entity:
         console.print("\n[bold red]Entity ID required.[/]\n")
         raise typer.Exit(1)
     data = get_solr(update=False)
     response = data.get_association_counts(entity)
     counts = AssociationCountList(items=response)
     format_output(fmt, counts, output)
+
+
+@solr_app.command("association-table")
+def association_table(
+    entity: str = typer.Argument(..., help="The entity to get associations for"),
+    association_type: AssociationTypeEnum = typer.Argument(
+        ..., help="The association type to get associations for"
+    ),
+    q: str = typer.Option(None, "--query", "-q"),
+    limit: int = typer.Option(5, "--limit", "-l"),
+    offset: int = typer.Option(0, "--offset"),
+    fmt: str = typer.Option(
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
+    ),
+    output: str = typer.Option(
+        None, "--output", "-o", help="The path to the output file"
+    ),
+):
+    data = get_solr(update=False)
+    response = data.get_association_table(
+        entity, association_type, q=q, limit=limit, offset=offset
+    )
+    format_output(fmt, response, output)
```

### Comparing `monarch_py-0.7.3/src/monarch_py/sql_cli.py` & `monarch_py-0.8.0/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.8.0/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.8.0/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/src/monarch_py/utils/utils.py` & `monarch_py-0.8.0/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.3/PKG-INFO` & `monarch_py-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.7.3
+Version: 0.8.0
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

