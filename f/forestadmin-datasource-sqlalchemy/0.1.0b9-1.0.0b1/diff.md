# Comparing `tmp/forestadmin_datasource_sqlalchemy-0.1.0b9.tar.gz` & `tmp/forestadmin_datasource_sqlalchemy-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_sqlalchemy-0.1.0b9.tar", max compression
+gzip compressed data, was "forestadmin_datasource_sqlalchemy-1.0.0b1.tar", max compression
```

## Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9.tar` & `forestadmin_datasource_sqlalchemy-1.0.0b1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0        0 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/README.md
--rw-r--r--   0        0        0      131 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/__init__.py
--rw-r--r--   0        0        0    12141 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/datasource.py
--rw-r--r--   0        0        0     1536 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/interfaces.py
--rw-r--r--   0        0        0        0 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/__init__.py
--rw-r--r--   0        0        0     5957 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/aggregation.py
--rw-r--r--   0        0        0     5981 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/model_converter.py
--rw-r--r--   0        0        0    10070 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/query_factory.py
--rw-r--r--   0        0        0     2916 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
--rw-r--r--   0        0        0      379 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/relationships.py
--rw-r--r--   0        0        0     6934 2022-12-07 16:21:13.507432 forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/type_converter.py
--rw-r--r--   0        0        0     1497 2022-12-07 16:21:32.936568 forestadmin_datasource_sqlalchemy-0.1.0b9/pyproject.toml
--rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-0.1.0b9/setup.py
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-0.1.0b9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11076 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/collections.py
+-rw-r--r--   0        0        0     3045 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/datasource.py
+-rw-r--r--   0        0        0      612 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/exceptions.py
+-rw-r--r--   0        0        0     1923 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/interfaces.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0     5956 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/aggregation.py
+-rw-r--r--   0        0        0     6235 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/model_converter.py
+-rw-r--r--   0        0        0    10207 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/query_factory.py
+-rw-r--r--   0        0        0     2943 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
+-rw-r--r--   0        0        0      519 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/relationships.py
+-rw-r--r--   0        0        0     7029 2023-07-21 14:35:50.675956 forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/type_converter.py
+-rw-r--r--   0        0        0     1808 2023-07-21 14:36:13.769010 forestadmin_datasource_sqlalchemy-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-1.0.0b1/PKG-INFO
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/datasource.py` & `forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/collections.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,48 @@
-import zoneinfo
+import sys
 from collections import defaultdict
 from datetime import datetime
-from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
-from forestadmin.datasource_sqlalchemy.interfaces import BaseSqlAlchemyCollection, BaseSqlAlchemyCollectionFactory
+if sys.version_info >= (3, 9):
+    import zoneinfo
+else:
+    from backports import zoneinfo
+
+from forestadmin.agent_toolkit.utils.context import User
+from forestadmin.datasource_sqlalchemy.exceptions import SqlAlchemyCollectionException, handle_sqlalchemy_error
+from forestadmin.datasource_sqlalchemy.interfaces import (
+    BaseSqlAlchemyCollection,
+    BaseSqlAlchemyCollectionFactory,
+    BaseSqlAlchemyDatasource,
+)
 from forestadmin.datasource_sqlalchemy.utils.model_converter import CollectionFactory
 from forestadmin.datasource_sqlalchemy.utils.query_factory import QueryFactory
 from forestadmin.datasource_sqlalchemy.utils.record_serializer import (
     aggregations_to_records,
     instances_to_records,
     projections_to_records,
 )
 from forestadmin.datasource_sqlalchemy.utils.relationships import Relationships, merge_relationships
-from forestadmin.datasource_toolkit.datasources import Datasource, DatasourceException
 from forestadmin.datasource_toolkit.interfaces.actions import ActionField, ActionResult
-from forestadmin.datasource_toolkit.interfaces.fields import (
-    FieldType,
-    ManyToMany,
-    ManyToOne,
-    PrimitiveType,
-    RelationAlias,
-)
+from forestadmin.datasource_toolkit.interfaces.chart import Chart
+from forestadmin.datasource_toolkit.interfaces.fields import PrimitiveType, RelationAlias
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import AggregateResult, Aggregation
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from forestadmin.datasource_toolkit.validations.type_getter import TypeGetter
 from sqlalchemy import Table
 from sqlalchemy import column as SqlAlchemyColumn
 from sqlalchemy.engine import Dialect
-from sqlalchemy.exc import SQLAlchemyError
-from sqlalchemy.orm import Mapper, RelationshipProperty, sessionmaker
-
-
-class SqlAlchemyCollectionException(DatasourceException):
-    pass
-
-
-def handle_sqlalchemy_error(fn: Callable[..., Awaitable[Any]]):
-    async def wrapped(self: Any, *args: Any, **kwargs: Any) -> Any:
-        try:
-            return await fn(self, *args, **kwargs)
-        except SQLAlchemyError as e:
-            raise SqlAlchemyCollectionException(str(e))
-
-    return wrapped
+from sqlalchemy.orm import Mapper, RelationshipProperty
+from sqlalchemy.sql import Alias, alias
 
 
 class SqlAlchemyCollectionFactory(BaseSqlAlchemyCollectionFactory):
     def __init__(self, collection: "SqlAlchemyCollection"):
         self._collection = collection
 
     @property
@@ -71,33 +62,34 @@
         if self.collection.model:
             try:
                 return self.collection.model(**data)  # type: ignore
             except TypeError as e:
                 unknown_fields = self._unknown_fields(data)
                 if unknown_fields:
                     raise SqlAlchemyCollectionException(
-                        f'Unknow fields "{unknown_fields}" for the model "{self.collection.model.__class__.__name__}"'
+                        f'Unknown fields "{unknown_fields}" for the model "{self.collection.model.__class__.__name__}"'
                     )
                 raise e
         raise
 
 
 class SqlAlchemyCollection(BaseSqlAlchemyCollection):
     def __init__(
         self,
         name: str,
-        datasource: "SqlAlchemyDatasource",
+        datasource: BaseSqlAlchemyDatasource,
         table: Table,
         mapper: Optional[Mapper] = None,
     ):
         super(SqlAlchemyCollection, self).__init__(name, datasource)
         self._table = table
         self._mapper = mapper
         self._name = name
         self._factory = SqlAlchemyCollectionFactory(self)
+        self._aliases: Dict[str, Alias] = {}
         schema = CollectionFactory.build(self.table, self.mapper)
         self.add_fields(schema["fields"])
 
     @property
     def table(self) -> Table:
         return self._table
 
@@ -111,80 +103,92 @@
             return self.mapper.class_
         return None
 
     @property
     def factory(self) -> SqlAlchemyCollectionFactory:
         return self._factory
 
-    def get_column(self, name: str) -> SqlAlchemyColumn:
+    def get_column(self, name: str, alias_: Optional[Alias] = None) -> SqlAlchemyColumn:
+        mapper = self.mapper
+        if alias_ is not None:
+            mapper = alias_
         try:
-            return self.mapper.columns[name]  # type: ignore
+            return mapper.columns[name]  # type: ignore
         except KeyError:
-            raise SqlAlchemyCollectionException(f"Unkown field '{name}' for the collection '{self.name}'")
+            raise SqlAlchemyCollectionException(f"Unknown field '{name}' for the collection '{self.name}'")
 
     def _get_relationship(self, name: str) -> RelationshipProperty:
         try:
             return self.mapper.relationships[name]  # type: ignore
         except KeyError:
-            raise SqlAlchemyCollectionException(f"Unkown relationship '{name}' for the collection '{self.name}'")
+            raise SqlAlchemyCollectionException(f"Unknown relationship '{name}' for the collection '{self.name}'")
 
-    def get_columns(self, projection: Projection, level: int = 0) -> Tuple[List[SqlAlchemyColumn], Relationships]:
+    def get_columns(
+        self, projection: Projection, level: int = 0, alias_: Optional[Alias] = None
+    ) -> Tuple[List[SqlAlchemyColumn], Relationships]:
         relationships: Relationships = defaultdict(list)
-        columns: List[SqlAlchemyColumn] = [self.get_column(column) for column in projection.columns]
+        columns: List[SqlAlchemyColumn] = [self.get_column(column, alias_) for column in projection.columns]
         nested_columns, nested_relationships = self._get_related_column(projection, level)
         columns.extend(nested_columns)
         relationships = merge_relationships(relationships, nested_relationships)
         return columns, relationships
 
+    def _get_alias(self, mapper: Mapper, name: str):
+        alias_name = f"alias_{name}"
+        if alias_name not in self._aliases:
+            self._aliases[alias_name] = alias(mapper, alias_name)
+        return self._aliases[alias_name]
+
     def _get_related_column(
         self, projection: Projection, level: int = 0
     ) -> Tuple[List[SqlAlchemyColumn], Relationships]:
         relationships: Dict[int, List[SqlAlchemyColumn]] = defaultdict(list)
         columns: List[SqlAlchemyColumn] = []
         for related_field_name, related_projection in projection.relations.items():
-            relationships[level].append(self._get_relationship(related_field_name).class_attribute)  # type: ignore
             related_field: RelationAlias = cast(RelationAlias, self.get_field(related_field_name))
             related_collection = self.datasource.get_collection(related_field["foreign_collection"])
-            nested_columns, nested_relationships = related_collection.get_columns(related_projection, level + 1)
+            alias_: Alias = self._get_alias(related_collection.mapper, related_field_name)  # type: ignore
+            nested_columns, nested_relationships = related_collection.get_columns(related_projection, level + 1, alias_)
             columns.extend(nested_columns)
+
+            relationship = self._get_relationship(related_field_name)
+            relationships[level].append((alias_, relationship.class_attribute))  # type: ignore
+
             merge_relationships(relationships, nested_relationships)
         return columns, relationships
 
-    def _normalize_projection(self, projection: Projection):
+    def _normalize_projection(self, projection: Projection, prefix: str = "") -> Projection:
         # needed to be compliant with the orm result orm
-        normalized_projection = projection.columns
+        normalized_projection = [f"{prefix}{col}" for col in projection.columns]
         for parent_field, child_fields in projection.relations.items():
-            for field in cast(List[str], child_fields):
-                normalized_projection.append(f"{parent_field}:{field}")
+            normalized_projection.extend(self._normalize_projection(child_fields, f"{prefix}{parent_field}:"))
         return Projection(*normalized_projection)
 
-    async def execute(self, name: str, data: RecordsDataAlias, filter: Optional[Filter]) -> ActionResult:
-        return await super().execute(name, data, filter)
-
     async def aggregate(
         self,
+        caller: User,
         filter: Optional[Filter],
         aggregation: Aggregation,
         limit: Optional[int] = None,
     ) -> List[AggregateResult]:
         with self.datasource.Session.begin() as session:  #  type: ignore
             dialect: Dialect = session.bind.dialect  #  type: ignore
             filter = cast(Filter, self._cast_filter(filter)) or None
             query = QueryFactory.build_aggregate(dialect, self, filter, aggregation, limit)
             res: List[Dict[str, Any]] = session.execute(query)  #  type: ignore
             return aggregations_to_records(res)
 
     @handle_sqlalchemy_error
-    async def create(self, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
+    async def create(self, caller: User, data: List[RecordsDataAlias]) -> List[RecordsDataAlias]:
         with self.datasource.Session.begin() as session:  #  type: ignore
             instances = QueryFactory.create(self, data)
             session.bulk_save_objects(instances, return_defaults=True)  # type: ignore
             return instances_to_records(self, instances)
 
-    async def update(self, filter: Optional[Filter], patch: RecordsDataAlias) -> None:
+    async def update(self, caller: User, filter: Optional[Filter], patch: RecordsDataAlias) -> None:
         with self.datasource.Session.begin() as session:  #  type: ignore
             query = QueryFactory.update(self, filter, patch)
             session.execute(query)  # type: ignore
 
     def _cast_condition_tree(self, tree: ConditionTree) -> ConditionTree:
         if isinstance(tree, ConditionTreeLeaf):
             if TypeGetter.get(tree.value, None) == PrimitiveType.DATE:
@@ -201,73 +205,31 @@
     def _cast_filter(self, filter: Union[Filter, PaginatedFilter, None]) -> Union[Filter, PaginatedFilter, None]:
         if filter and filter.condition_tree:
             filter = filter.override(
                 {"condition_tree": filter.condition_tree.replace(self._cast_condition_tree)}  # type: ignore
             )
         return filter
 
-    async def list(self, filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
+    async def list(self, caller: User, filter: PaginatedFilter, projection: Projection) -> List[RecordsDataAlias]:
         with self.datasource.Session.begin() as session:  #  type: ignore
-            projection = self._normalize_projection(projection)
+            normalized_projection = self._normalize_projection(projection)
             filter = cast(PaginatedFilter, self._cast_filter(filter))
-            query = QueryFactory.build_list(self, filter, projection)
+            query = QueryFactory.build_list(self, filter, normalized_projection)
             res = session.execute(query).all()  #  type: ignore
-            records = projections_to_records(projection, res, filter.timezone)  # type: ignore
+            records = projections_to_records(normalized_projection, res, filter.timezone)  # type: ignore
             return records
 
-    async def delete(self, filter: Optional[Filter]) -> None:
+    async def delete(self, caller: User, filter: Optional[Filter]) -> None:
         with self.datasource.Session.begin() as session:  #  type: ignore
             query = QueryFactory.delete(self, filter)
             session.execute(query)  # type: ignore
 
     async def get_form(
-        self, name: str, data: Optional[RecordsDataAlias], filter: Optional[Filter]
+        self, caller: User, name: str, data: Optional[RecordsDataAlias], filter: Optional[Filter]
     ) -> List[ActionField]:
-        return await super().get_form(name, data, filter)
-
+        return await super().get_form(caller, name, data, filter)
 
-class SqlAlchemyDatasource(Datasource[SqlAlchemyCollection]):
-    def __init__(self, Base: Any) -> None:
-        super().__init__()
-        self._base = Base
-        self.Session = sessionmaker(self._base.metadata.bind)  # type: ignore
-        self._create_collections()
-
-    def build_mappers(self) -> Dict[str, Mapper]:
-        mappers: Dict[str, Mapper] = {}
-        for mapper in self._base.registry.mappers:
-            mappers[mapper.persist_selectable.name] = mapper
-        return mappers
+    async def execute(self, caller: User, name: str, data: RecordsDataAlias, filter: Optional[Filter]) -> ActionResult:
+        return await super().execute(caller, name, data, filter)
 
-    def _create_secondary_collection(self, table: Any):
-        try:
-            collection = self.get_collection(table.name)
-        except DatasourceException:
-            Secondary = type(str(table.name), tuple(), {})  # type: ignore
-            mapper = self._base.registry.map_imperatively(Secondary, table)
-            collection = SqlAlchemyCollection(table.name, self, table, mapper)
-            self.add_collection(collection)
-        return collection
-
-    def _create_secondary_relation(
-        self,
-        collection: SqlAlchemyCollection,
-        related_collection_name: str,
-        many_to_many: ManyToMany,
-    ):
-        collection.add_field(
-            related_collection_name.lower(),
-            ManyToOne(
-                foreign_collection=related_collection_name,
-                foreign_key=many_to_many["origin_key"],
-                foreign_key_target=many_to_many["origin_key_target"],
-                type=FieldType.MANY_TO_ONE,
-            ),
-        )
-        return many_to_many["foreign_collection"].lower()
-
-    def _create_collections(self):
-        mappers = self.build_mappers()
-        for table in self._base.metadata.sorted_tables:
-            if table.name in mappers:
-                collection = SqlAlchemyCollection(table.name, self, table, mappers[table.name])
-                self.add_collection(collection)
+    async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
+        return await super().render_chart(caller, name, record_id)
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/interfaces.py` & `forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/interfaces.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 import abc
 from typing import Any, Callable, List, Optional, Tuple
 
 from forestadmin.datasource_sqlalchemy.utils.relationships import Relationships
 from forestadmin.datasource_toolkit.collections import Collection
+from forestadmin.datasource_toolkit.datasources import Datasource
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from sqlalchemy import Table
 from sqlalchemy import column as SqlAlchemyColumn
 from sqlalchemy.orm import Mapper
 from typing_extensions import Self
 
 
 class BaseSqlAlchemyCollectionFactory(abc.ABC):
     @abc.abstractmethod
     def init_instance(self, data: RecordsDataAlias) -> "BaseSqlAlchemyCollection":
-        pass
+        """instantiate model class from raw data"""
 
 
 class BaseSqlAlchemyCollection(Collection, abc.ABC):
     @abc.abstractmethod
     def get_column(self, name: str) -> Self:
-        pass
+        """return column name 'name'"""
 
     @abc.abstractmethod
     def _get_related_column(
         self, projection: Projection, level: int = 0
     ) -> Tuple[List[SqlAlchemyColumn], Relationships]:
-        pass
+        """return (columns, relationships)"""
 
     @abc.abstractmethod
     def get_columns(self, projection: Projection, level: int = 0) -> Tuple[List[SqlAlchemyColumn], Relationships]:
-        pass
+        """return (columns, relationships)"""
 
     @abc.abstractproperty
     def table(self) -> Table:  # type: ignore
-        pass
+        """return table of this collection"""
 
     @abc.abstractproperty
     def mapper(self) -> Optional[Mapper]:
-        pass
+        """return table mapper"""
 
     @abc.abstractproperty
     def model(self) -> Optional[Callable[[Any], Any]]:
-        pass
+        """return model of the collection"""
 
     @abc.abstractproperty
     def factory(self) -> BaseSqlAlchemyCollectionFactory:  # type: ignore
-        pass
+        """return collection factory"""
+
+
+class BaseSqlAlchemyDatasource(Datasource[Collection], abc.ABC):
+    pass
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/aggregation.py` & `forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 class AggregationFactoryException(DatasourceToolkitException):
     pass
 
 
 class AggregationFactory:
-
     LABEL = "__aggregate__"
     GROUP_LABEL = "__grouped__"
 
     MAPPING = {
         Aggregator.COUNT: func.count,
         Aggregator.MIN: func.min,
         Aggregator.MAX: func.max,
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/model_converter.py` & `forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/model_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Any, Dict, List, Optional
 
 from forestadmin.datasource_sqlalchemy.utils.type_converter import Converter as TypeConverter
 from forestadmin.datasource_sqlalchemy.utils.type_converter import FilterOperator
 from forestadmin.datasource_toolkit.interfaces.fields import (
     Column,
     FieldType,
@@ -10,15 +11,15 @@
     OneToMany,
     OneToOne,
     Operator,
     RelationAlias,
     Validation,
 )
 from forestadmin.datasource_toolkit.interfaces.models.collections import CollectionSchema
-from sqlalchemy import Enum, Table
+from sqlalchemy import ColumnDefault, Enum, Table
 from sqlalchemy.orm import Mapper
 from sqlalchemy.sql.schema import Column as SqlAlchemyColumn
 
 
 class ColumnFactory:
     @staticmethod
     def _build_enum_values(column: SqlAlchemyColumn) -> Optional[List[str]]:
@@ -46,20 +47,27 @@
             )
 
         return validations
 
     @classmethod
     def build(cls, column: SqlAlchemyColumn) -> Column:
         column_type = TypeConverter.convert(column.type)  # type: ignore
+
+        default_value = column.default.arg if isinstance(column.default, ColumnDefault) else column.default
+        try:
+            json.dumps(default_value)
+        except TypeError:  # not JSON Serializable
+            default_value = None
+
         return {
             "column_type": column_type,
             "is_primary_key": column.primary_key,  # type: ignore
             "is_read_only": cls._build_is_read_only(column),
-            "default_value": column.default,  # type: ignore
-            "is_sortable": None,
+            "default_value": default_value,
+            "is_sortable": True,
             "validations": cls._build_validations(column),
             "filter_operators": FilterOperator.get_for_type(column_type),
             "enum_values": cls._build_enum_values(column),
             "type": FieldType.COLUMN,
         }
 
 
@@ -145,9 +153,8 @@
                     elif relationship.secondary is not None:  # type: ignore
                         relation = cls._build_many_to_many(model, relationship)
                     else:
                         relation = cls._build_one_to_many(relationship)
 
                     if relation:
                         fields[relationship.key] = relation  # type: ignore
-
         return {"actions": {}, "fields": fields, "searchable": False, "segments": []}
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/query_factory.py` & `forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/query_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 
 class ConditionTreeFactoryException(DatasourceToolkitException):
     pass
 
 
 class ConditionTreeFactory:
-
     AGGREGATORS = {Aggregator.AND: and_, Aggregator.OR: or_}
 
     @classmethod
     def _build_leaf_condition(cls, collection: BaseSqlAlchemyCollection, leaf: ConditionTreeLeaf) -> Tuple[Any, Any]:
         projection = leaf.projection
         columns, relationships = collection.get_columns(projection)
         operator = FilterOperator.get_operator(columns, leaf.operator)
@@ -101,15 +100,18 @@
 
 class PaginatedFilterFactory:
     @staticmethod
     def get_order_by(collection: BaseSqlAlchemyCollection, filter: PaginatedFilter) -> Tuple[List[Any], Relationships]:
         relationships: Relationships = defaultdict(list)
         order_clauses: List[Any] = []
         for sort in cast(List[PlainSortClause], filter.sort or []):
-            columns, nested_relationships = collection.get_columns(Projection(sort["field"]))
+            field = sort["field"]
+            if "." in field:
+                field = field.replace(".", ":")
+            columns, nested_relationships = collection.get_columns(Projection(field))
             relationships = merge_relationships(relationships, nested_relationships)
             if sort["ascending"]:
                 order_clauses.append(columns[0].asc())  # type: ignore
             else:
                 order_clauses.append(columns[0].desc())  # type: ignore
         return order_clauses, relationships
 
@@ -139,30 +141,29 @@
         collection: BaseSqlAlchemyCollection,
         filter: Optional[PaginatedFilter],
         columns: List[SqlAlchemyColumn],
         relationships: Optional[Relationships] = None,
     ):
         if not relationships:
             relationships = defaultdict(list)
-        query: Any = select(columns).select_from(collection.mapper)
+        query: Any = select(*columns).select_from(collection.mapper)
         if filter:
             options = PaginatedFilterFactory.build(collection, filter)
             relationships = merge_relationships(relationships, options.get("relationships", {}))
-
             if options.get("clauses") is not None:
                 query = query.where(options["clauses"])
             if options.get("order_by"):
                 query = query.order_by(*options.get("order_by"))
 
             if filter.page:
                 query = query.limit(filter.page.limit).offset(filter.page.skip)
 
         for level in sorted(relationships.keys()):
-            query = query.join(*relationships[level], isouter=True)
-
+            for relationship in relationships[level]:
+                query = query.join(*relationship)
         return query
 
     @classmethod
     def build_list(
         cls,
         collection: BaseSqlAlchemyCollection,
         filter: PaginatedFilter,
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/record_serializer.py` & `forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/record_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,13 +60,13 @@
         records.append(record)
     return records
 
 
 def aggregations_to_records(items: List[Dict[str, Any]]):
     records: List[AggregateResult] = []
     for item in items:
-        result = AggregateResult(value=item[AggregationFactory.LABEL], group={})
-        for key in item.keys():
+        result = AggregateResult(value=item._mapping[AggregationFactory.LABEL], group={})
+        for key in item._mapping.keys():
             if AggregationFactory.GROUP_LABEL in key:
-                result["group"][AggregationFactory.get_field_from_group_field_name(key)] = item[key]
+                result["group"][AggregationFactory.get_field_from_group_field_name(key)] = item._mapping[key]
         records.append(result)
     return records
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/forestadmin/datasource_sqlalchemy/utils/type_converter.py` & `forestadmin_datasource_sqlalchemy-1.0.0b1/forestadmin/datasource_sqlalchemy/utils/type_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 class ConverterException(DatasourceToolkitException):
     pass
 
 
 class Converter:
-
     TYPES: Dict[Type[sqltypes.TypeEngine], PrimitiveType] = {
         sqltypes.BigInteger: PrimitiveType.NUMBER,
         sqltypes.Boolean: PrimitiveType.BOOLEAN,
         sqltypes.CHAR: PrimitiveType.STRING,
         sqltypes.Date: PrimitiveType.DATE_ONLY,
         sqltypes.DateTime: PrimitiveType.DATE,
         sqltypes.DECIMAL: PrimitiveType.NUMBER,
@@ -45,15 +44,14 @@
         try:
             return cls.TYPES[_type.__class__]
         except KeyError:
             raise ConverterException(f'Type "{_type.__class__}" is unknown')
 
 
 class FilterOperator:
-
     COMMON_OPERATORS: Set[Operator] = {
         Operator.BLANK,
         Operator.EQUAL,
         Operator.MISSING,
         Operator.NOT_EQUAL,
         Operator.PRESENT,
     }
@@ -63,15 +61,17 @@
         Operator.NOT_EQUAL: "_not_equal_operator",
         Operator.BLANK: "_blank_operator",
         Operator.CONTAINS: "_contains_operator",
         Operator.NOT_CONTAINS: "_not_contains_operator",
         Operator.STARTS_WITH: "_starts_with_operator",
         Operator.ENDS_WITH: "_ends_with_operator",
         Operator.GREATER_THAN: "_greater_than_operator",
+        Operator.AFTER: "_greater_than_operator",
         Operator.LESS_THAN: "_less_than_operator",
+        Operator.BEFORE: "_less_than_operator",
         Operator.MISSING: "_missing_operator",
         Operator.PRESENT: "_present_operator",
         Operator.IN: "_in_operator",
         Operator.NOT_IN: "_not_in_operator",
         Operator.INCLUDES_ALL: "_includes_all",
     }
 
@@ -152,16 +152,15 @@
             meth = cls.OPERATORS[operator]
         except KeyError:
             raise ConverterException(f"Unable to handle the operator {operator}")
         else:
             return getattr(cls, meth)(columns[0])
 
     @classmethod
-    def get_for_type(cls, _type: ColumnAlias) -> set[Operator]:
-
+    def get_for_type(cls, _type: ColumnAlias) -> Set[Operator]:
         operators: Set[Operator] = set()
         if isinstance(_type, list):
             operators = {
                 *cls.COMMON_OPERATORS,
                 Operator.IN,
                 Operator.INCLUDES_ALL,
                 Operator.NOT_IN,
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/pyproject.toml` & `forestadmin_datasource_sqlalchemy-1.0.0b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-sqlalchemy"
-version = "0.1.0-beta.9"
+version = "1.0.0-beta.1"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
@@ -19,15 +19,17 @@
 upload_to_release = false
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
-forestadmin-datasource-toolkit = "^0.1.0-beta.9"
+sqlalchemy = "^1.4.44"
+forestadmin-datasource-toolkit = "^1.0.0-beta.1"
+forestadmin-agent-toolkit = "^1.0.0-beta.1"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
 [tool.poetry.group.test]
@@ -43,14 +45,15 @@
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "~=7.1"
 pytest-asyncio = "~=0.18"
 coverage = "~=6.5"
 freezegun = "~=1.2.0"
+pytest-cov = "^4.0.0"
 [[tool.poetry.group.test.dependencies.mock]]
 version = "4.0"
 python = "3.7"
 
 [tool.poetry.group.linter.dependencies]
 [[tool.poetry.group.linter.dependencies.flake8]]
 version = "~=5.0"
@@ -61,7 +64,15 @@
 python = ">=3.8.1"
 
 [tool.poetry.group.formatter.dependencies]
 black = "~=22.10"
 
 [tool.poetry.group.sorter.dependencies]
 isort = "~=3.6"
+
+[tool.poetry.group.test.dependencies.forestadmin-datasource-toolkit]
+path = "../datasource_toolkit"
+develop = true
+
+[tool.poetry.group.test.dependencies.forestadmin-agent-toolkit]
+path = "../agent_toolkit"
+develop = true
```

### Comparing `forestadmin_datasource_sqlalchemy-0.1.0b9/PKG-INFO` & `forestadmin_datasource_sqlalchemy-1.0.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-sqlalchemy
-Version: 0.1.0b9
+Version: 1.0.0b1
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0); python_version < "3.9"
-Requires-Dist: forestadmin-datasource-toolkit (>=0.1.0-beta.9,<0.2.0)
+Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
+Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.1,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.1,<2.0.0)
+Requires-Dist: sqlalchemy (>=1.4.44,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2023.0)
 Description-Content-Type: text/markdown
```

