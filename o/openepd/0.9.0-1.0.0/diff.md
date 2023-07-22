# Comparing `tmp/openepd-0.9.0.tar.gz` & `tmp/openepd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.9.0.tar", max compression
+gzip compressed data, was "openepd-1.0.0.tar", max compression
```

## Comparing `openepd-0.9.0.tar` & `openepd-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-06-09 16:35:21.066648 openepd-0.9.0/LICENSE
--rw-r--r--   0        0        0     2841 2023-06-09 16:35:21.066648 openepd-0.9.0/README.md
--rw-r--r--   0        0        0     3051 2023-06-09 16:35:21.066648 openepd-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     3640 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     4545 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    12287 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0    13712 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3813 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     2889 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     1137 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3342 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1519 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0        0 2023-06-09 16:35:21.070648 openepd-0.9.0/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-22 15:05:29.529160 openepd-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5813 2023-07-22 15:05:29.529160 openepd-1.0.0/README.md
+-rw-r--r--   0        0        0     3031 2023-07-22 15:05:29.529160 openepd-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-07-22 15:05:29.529160 openepd-1.0.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-07-22 15:05:29.529160 openepd-1.0.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:05:29.529160 openepd-1.0.0/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2023-07-22 15:05:29.529160 openepd-1.0.0/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2647 2023-07-22 15:05:29.529160 openepd-1.0.0/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2023-07-22 15:05:29.529160 openepd-1.0.0/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8325 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     5564 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     5386 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    13057 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0    16711 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3662 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     3205 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     1137 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3342 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1519 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0        0 2023-07-22 15:05:29.533160 openepd-1.0.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     6706 1970-01-01 00:00:00.000000 openepd-1.0.0/PKG-INFO
```

### Comparing `openepd-0.9.0/LICENSE` & `openepd-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.9.0/pyproject.toml` & `openepd-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [tool.poetry]
 name = "openepd"
-version = "0.9.0"
+version = "1.0.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
-maintainers = ["C-Change Labs <support@c-change-labs.com>"]
+maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 readme = "README.md"
 packages = [{include = "openepd", from = "src"}]
-exclude = ["**/test_*.py"]
+exclude = ["**/test_*.py", "**/tests/**"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pydantic = ">=1.10"
-email-validator = ">=2.0"
+pydantic = ">=1.10,<2.0"
+email-validator = ">=1.3.0"
 
 # Optional dependencies
 # lxml = { version = "~=4.9.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
 coverage = { version = "=6.5", extras = ["toml"] }
 pytest = "~=7.2"
 pytest-subtests = "~=0.4"
 pytest-cov = "~=4.0"
 teamcity-messages = ">=1.31"
+wheel = "~=0.40.0"
 
 # Dev tools
-#virtualenv = "<=20.23.0" # to avoid conflict with flake plugins
 black = "~=22.3"
 licenseheaders = "~=0.8"
 flake8 = "~=4.0"
 flake8-import-graph = "~=0.1.3"
 flake8-docstrings = "~=1.7.0"
 isort = "~=5.11"
 mypy = ">=1.0.1"
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.9.0"
+version = "1.0.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.9.0/src/openepd/__init__.py` & `openepd-1.0.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.9.0/src/openepd/__version__.py` & `openepd-1.0.0/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.9.0"
+VERSION = "1.0.0"
```

### Comparing `openepd-0.9.0/src/openepd/model/__init__.py` & `openepd-1.0.0/src/openepd/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.9.0/src/openepd/model/base.py` & `openepd-1.0.0/src/openepd/model/specs/concrete.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,89 +13,71 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Optional, Type, TypeVar
+from enum import StrEnum
 
-import pydantic
-from pydantic.generics import GenericModel
+import pydantic as pyd
 
-AnySerializable = int | str | bool | float | list | dict | pydantic.BaseModel | None
-TAnySerializable = TypeVar("TAnySerializable", bound=AnySerializable)
+from openepd.model.base import BaseOpenEpdSpec
 
 
-class BaseOpenEpdSchema(pydantic.BaseModel):
-    """Base class for all OpenEPD models."""
-
-    ext: dict[str, AnySerializable] | None = pydantic.Field(alias="ext", default=None)
-
-    class Config:
-        allow_mutation = True
-        validate_assignment = False
-        allow_population_by_field_name = True
-        use_enum_values = True
-
-    def has_values(self) -> bool:
-        """Return True if the model has any values."""
-        return len(self.dict(exclude_unset=True, exclude_none=True)) > 0
-
-    def set_ext_field(self, key: str, value: AnySerializable) -> None:
-        """Add an extension field to the model."""
-        if self.ext is None:
-            self.ext = {}
-        self.ext[key] = value
-
-    def set_ext_field_if_any(self, key: str, value: AnySerializable) -> None:
-        """Add an extension field to the model if the value is not None."""
-        if value is not None:
-            self.set_ext_field(key, value)
-
-    def get_ext_field(self, key: str, default: AnySerializable = None) -> AnySerializable | None:
-        """Get an extension field from the model."""
-        if self.ext is None:
-            return default
-        return self.ext.get(key, default)
-
-    def get_typed_ext_field(
-        self, key: str, target_type: Type[TAnySerializable], default: Optional[TAnySerializable] = None
-    ) -> TAnySerializable:
-        """
-        Get an extension field from the model and convert it to the target type.
-
-        :raise ValueError: if the value cannot be converted to the target type.
-        """
-        value = self.get_ext_field(key, default)
-        if issubclass(target_type, pydantic.BaseModel) and isinstance(value, dict):
-            return target_type.construct(**value)  # type: ignore
-        elif isinstance(value, target_type):
-            return value
-        raise ValueError(f"Cannot convert {value} to {target_type}")
-
-    @classmethod
-    def is_allowed_field_name(cls, field_name: str) -> bool:
-        """
-        Return True if the field name is defined in the module.
-
-        Both property name and aliases are checked.
-        """
-        if field_name in cls.__fields__:
-            return True
-        else:
-            for x in cls.__fields__.values():
-                if x.alias == field_name:
-                    return True
-        return False
-
-
-class BaseOpenEpdGenericSchema(GenericModel, BaseOpenEpdSchema):
-    """Base class for all OpenEPD generic models."""
-
-    pass
-
-
-class BaseOpenEpdSpec(BaseOpenEpdSchema):
-    """Base class for all OpenEPD specs."""
-
-    pass
+class CmuWeightClassification(StrEnum):
+    """Concrete Masonry Unit weight classification."""
+
+    Normal = "Normal"
+    """Normal weight CMU has a density of 125 lbs/cu. ft."""
+    Medium = "Medium"
+    """Medium weight CMU has a density of 105-125 lbs/cu. ft."""
+    Light = "Light"
+    """Lightweight CMU has a density less than 105 lbs/cu. ft."""
+
+
+class CmuOptions(BaseOpenEpdSpec):
+    """Concrete Masonry Unit options."""
+
+    load_bearing: bool | None = pyd.Field(
+        description="Load-Bearing. CMUs intended to be loadbearing, rather than simply cosmetic",
+        example=True,
+        default=None,
+    )
+    aerated_concrete: bool | None = pyd.Field(
+        description="AAC Aerated Concrete. Aerated Autoclaved Concrete, a foam concrete.", example=True, default=None
+    )
+    insulated: bool | None = pyd.Field(
+        description="Insulated. CMUs with integral insulation", example=True, default=None
+    )
+    sound_absorbing: bool | None = pyd.Field(
+        description="Sound Absorbing. CMUs structured for sound absorbtion", example=True, default=None
+    )
+    white: bool | None = pyd.Field(
+        description="White. CMU using white cement and light-colored aggregate", example=True, default=None
+    )
+    recycled_aggregate: bool | None = pyd.Field(
+        description="Recycled aggregate. CMU using primarily reycled aggregates", example=True, default=None
+    )
+    groundface: bool | None = pyd.Field(
+        description="Ground Face. Ground or Honed facing, typically for improved appearance", example=True, default=None
+    )
+    splitface: bool | None = pyd.Field(
+        description="Splitface. Rough surface texture via splitting; aggregate can be seen", example=True, default=None
+    )
+    smoothface: bool | None = pyd.Field(
+        description="Smooth Face. Standard smooth-faced blocks", example=True, default=None
+    )
+    slumpstone: bool | None = pyd.Field(
+        description="Slumpstone. A slightly rounded, random distortion with the look of rustic adobe.",
+        example=True,
+        default=None,
+    )
+
+
+class CmuSpec(BaseOpenEpdSpec):
+    """Standardized Concrete Masonry Unit-specific extension for OpenEPD."""
+
+    strength: str = pyd.Field(description="Compressive strength", example="4000 psi")
+    options: CmuOptions = pyd.Field(
+        description="Options for CMU. List of true/false properties", default_factory=CmuOptions
+    )
```

### Comparing `openepd-0.9.0/src/openepd/model/common.py` & `openepd-1.0.0/src/openepd/model/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -69,14 +69,33 @@
     link: pyd.AnyUrl | None = pyd.Field(
         description="Link to this object's OpenEPD declaration. "
         "An OpenIndustryEPD or OpenLCI link is also acceptable.",
         default=None,
     )
 
 
+class LatLng(BaseOpenEpdSchema):
+    """A latitude and longitude."""
+
+    lat: float = pyd.Field(description="Latitude", example=47.6062)
+    lng: float = pyd.Field(description="Longitude", example=-122.3321)
+
+
+class Location(BaseOpenEpdSchema):
+    """A location on the Earth's surface."""
+
+    pluscode: str | None = pyd.Field(default=None, description="Open Location code of this location")
+    latlng: LatLng | None = pyd.Field(default=None, description="Latitude and longitude of this location")
+    address: str | None = pyd.Field(default=None, description="Text address, preferably geocoded")
+    country: str | None = pyd.Field(default=None, description="2-alpha country code")
+    jurisdiction: str | None = pyd.Field(
+        default=None, description="Province, State, or similar subdivision below the level of a country"
+    )
+
+
 class WithAttachmentsMixin(BaseModel):
     """Mixin for objects that can have attachments."""
 
     attachments: dict[Annotated[str, pyd.Field(max_length=200)], pyd.AnyUrl] | None = pyd.Field(
         description="Dict of URLs relevant to this entry",
         example={
             "Contact Us": "https://www.c-change-labs.com/en/contact-us/",
```

### Comparing `openepd-0.9.0/src/openepd/model/epd.py` & `openepd-1.0.0/src/openepd/model/epd.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
-from typing import Annotated, Literal
+from typing import Annotated
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Amount, Ingredient, WithAltIdsMixin, WithAttachmentsMixin
 from openepd.model.lcia import Impacts, OutputFlowSet, ResourceUseSet
 from openepd.model.org import Org, Plant
@@ -31,24 +31,25 @@
 from openepd.model.standard import Standard
 
 
 class Epd(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent an EPD."""
 
     # TODO: Add validator for open-xpd-uuid on this field
-    id: str = pyd.Field(
+    id: str | None = pyd.Field(
         description="The unique ID for this EPD.  To ensure global uniqueness, should be registered at "
         "open-xpd-uuid.cqd.io/register or a coordinating registry.",
         example="1u7zsed8",
+        default=None,
     )
-    doctype: Literal["OpenEPD", "ILCD_EPD"] = pyd.Field(
+    doctype: str = pyd.Field(
         description='Describes the type and schema of the document. Must always always read "openEPD".',
         default="OpenEPD",
     )
-    product_name: str = pyd.Field(
+    product_name: str | None = pyd.Field(
         max_length=200, description="The name of the product described by this EPD", example="Mix 12345AC"
     )
     product_sku: str | None = pyd.Field(
         max_length=200, description="Unique stock keeping identifier assigned by manufacturer"
     )
     product_description: str | None = pyd.Field(
         max_length=2000,
@@ -60,18 +61,19 @@
     )
     product_image_small: pyd.AnyUrl | None = pyd.Field(
         description="Pointer to image illustrating the product, which is no more than 200x200 pixels", default=None
     )
     product_image: pyd.AnyUrl | None = pyd.Field(
         description="pointer to image illustrating the product no more than 10MB", default=None
     )
-    version: pyd.PositiveInt = pyd.Field(
+    version: pyd.PositiveInt | None = pyd.Field(
         description="Version of this document. The document's issuer should increment it anytime even a single "
         "character changes, as this value is used to determine the most recent version.",
         example=1,
+        default=None,
     )
     language: str | None = pyd.Field(
         min_length=2,
         max_length=2,
         strip_whitespace=True,
         description="Language this EPD is captured in, as an ISO 639-1 code",
         example="en",
@@ -85,19 +87,28 @@
         "number of required fields, to allow for multiple systems to coordinate "
         "incomplete EPDs.",
     )
     declaration_url: pyd.AnyUrl | None = pyd.Field(
         description="Link to data object on original registrar's site",
         example="https://epd-online.com/EmbeddedEpdList/Download/6029",
     )
-    # ilcd_uuid: str | None = pyd.Field(description="An optional UUID (for use with ILCD and similar systems)")
     manufacturer: Org | None = pyd.Field(
         description="JSON object for declaring Org. Sometimes called the "
         '"Declaration Holder" or "Declaration Owner".'
     )
+    epd_developer: Org | None = pyd.Field(
+        description="The organization responsible for the underlying LCA (and subsequent summarization as EPD).",
+        default=None,
+    )
+    epd_developer_email: pyd.EmailStr | None = pyd.Field(
+        default=None,
+        example="john.doe@we-do-lca.com",
+        description="Email contact for inquiries about development of this EPD. "
+        "This must be an email which can be publicly shared.",
+    )
     plants: list[Plant] = pyd.Field(
         max_items=32,
         description="List of object(s) for one or more plant(s) that this declaration applies to.",
         default_factory=list,
     )
     program_operator: Org | None = pyd.Field(description="JSON object for program operator Org")
     program_operator_doc_id: str | None = pyd.Field(
@@ -109,14 +120,17 @@
     third_party_verifier: Org | None = pyd.Field(
         description="JSON object for Org that performed a critical review of the EPD data"
     )
     third_party_verification_url: pyd.AnyUrl | None = pyd.Field(
         description="Optional link to a verification statement.",
         example="https://we-verify-epds.com/en/letters/123-456.789b.pdf",
     )
+    third_party_verifier_email: pyd.EmailStr | None = pyd.Field(
+        description="Email address of the third party verifier", example="john.doe@example.com", default=None
+    )
     date_of_issue: datetime.date | None = pyd.Field(
         example=datetime.date(day=11, month=9, year=2019),
         description="Date the EPD was issued. This should be the first day on which the EPD is valid.",
     )
     valid_until: datetime.date | None = pyd.Field(
         example=datetime.date(day=11, month=9, year=2028),
         description="Last date the EPD is valid on, including any extensions.",
@@ -208,14 +222,15 @@
         default_factory=Specs,
         description="Data structure(s) describing performance specs of product. Unique for each material type.",
     )
     includes: list[Ingredient] = pyd.Field(
         max_items=255,
         description="List of JSON objects pointing to product components. "
         "Each one should be an EPD or digitized LCI process.",
+        default_factory=list,
     )
     lca_discussion: str | None = pyd.Field(
         max_length=20000,
         description="""A rich text description containing information for experts reviewing the EPD contents. 
     Text descriptions required by ISO 14025, ISO 21930, EN 15804,, relevant PCRs, or program instructions and which do not 
     have specific openEPD fields should be entered here.  This field may be large, and may contain multiple sections 
     separated by github flavored markdown formatting.""",
@@ -236,7 +251,12 @@
     # Use Conditions
 
     Use-stage environmental impacts of flooring products during building operations depend on product cleaning assumptions. 
     Information on cleaning frequency and cleaning products shall be provided based on the manufacturer’s recommendations. 
     In the absence of primary data, cleaning assumptions shall be documented.
     """,
     )
+
+    @classmethod
+    def get_asset_type(cls) -> str | None:
+        """Return the asset type of this class (see BaseOpenEpdSchema.get_asset_type for details)."""
+        return "epd"
```

### Comparing `openepd-0.9.0/src/openepd/model/org.py` & `openepd-1.0.0/src/openepd/model/org.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,66 +18,75 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Annotated, Optional
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import WithAltIdsMixin, WithAttachmentsMixin
-
-
-class Contact(BaseOpenEpdSchema):  # TODO: NEW Object, not in the spec
-    """Contact information of a person or organization."""
-
-    email: pyd.EmailStr | None = pyd.Field(description="Email", example="contact@c-change-labs.com", default=None)
-    phone: str | None = pyd.Field(description="Phone number", example="+15263327352", default=None)
-    website: pyd.AnyUrl | None = pyd.Field(
-        description="Url of the website", example="http://buildingtransparency.org", default=None
-    )
-    address: str | None = pyd.Field(description="Address", example="123 Main St, San Francisco, CA 94105", default=None)
+from openepd.model.common import Location, WithAltIdsMixin, WithAttachmentsMixin
 
 
 class Org(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent an organization."""
 
-    web_domain: str = pyd.Field(
-        description="A web domain owned by organization. Typically is the org's home website address",
+    web_domain: str | None = pyd.Field(
+        description="A web domain owned by organization. Typically is the org's home website address", default=None
+    )
+    name: str | None = pyd.Field(
+        max_length=200,
+        description="Common name for organization",
+        example="C Change Labs",
+        default=None,
     )
-    name: str = pyd.Field(max_length=200, description="Common name for organization", example="C Change Labs")
     alt_names: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
         description="List of other names for organization",
         example=["C-Change Labs", "C-Change Labs inc."],
         default=None,
     )
     # TODO: NEW field, not in the spec
-    contacts: Contact | None = pyd.Field(description="Contact information of the organization", default=None)
     owner: Optional["Org"] = pyd.Field(description="Organization that controls this organization", default=None)
     subsidiaries: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
         description="Organizations controlled by this organization",
         example=["cqd.io", "supplychaincarbonpricing.org"],
         default=None,
     )
+    hq_location: Location | None = pyd.Field(
+        default=None,
+        description="Location of a place of business, prefereably the corporate headquarters.",
+    )
 
 
 class Plant(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent a manufacturing plant."""
 
     # TODO: Add proper validator
-    id: str = pyd.Field(
+    id: str | None = pyd.Field(
         description="Plus code (aka Open Location Code) of plant's location and "
         "owner's web domain joined with `.`(dot).",
         example="865P2W3V+3W.interface.com",
         alias="pluscode",
+        default=None,
     )
     owner: Org | None = pyd.Field(description="Organization that owns the plant", default=None)
-    name: str = pyd.Field(
-        max_length=200, description="Manufacturer's name for plant. Recommended < 40 chars", example="Dalton, GA"
+    name: str | None = pyd.Field(
+        max_length=200,
+        description="Manufacturer's name for plant. Recommended < 40 chars",
+        example="Dalton, GA",
+        default=None,
     )
-    address: str = pyd.Field(
+    address: str | None = pyd.Field(
         max_length=200,
+        default=None,
         description="Text address, preferably geocoded",
         example="1503 Orchard Hill Rd, LaGrange, GA 30240, United States",
     )
-    contact_email: pyd.EmailStr | None = pyd.Field(description="Email contact", example="info@interface.com")
+    contact_email: pyd.EmailStr | None = pyd.Field(
+        description="Email contact", example="info@interface.com", default=None
+    )
+
+    @classmethod
+    def get_asset_type(cls) -> str | None:
+        """Return the asset type of this class (see BaseOpenEpdSchema.get_asset_type for details)."""
+        return "org"
 
     class Config(BaseOpenEpdSchema.Config):
         allow_population_by_field_name = True
```

### Comparing `openepd-0.9.0/src/openepd/model/pcr.py` & `openepd-1.0.0/src/openepd/model/pcr.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,48 +26,59 @@
 from openepd.model.common import WithAltIdsMixin, WithAttachmentsMixin
 from openepd.model.org import Org
 
 
 class Pcr(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent a PCR (Product Category Rules)."""
 
-    id: str = pyd.Field(
+    id: str | None = pyd.Field(
         description="The unique ID for this PCR.  To ensure global uniqueness, should be registered "
         "at open-xpd-uuid.cqd.io/register or a coordinating registry.",
         example="ec3xpgq2",
+        default=None,
     )
     issuer: Org | None = pyd.Field(description="Organization issuing this PCR", default=None)
     issuer_doc_id: str | None = pyd.Field(
         max_length=40,
+        default=None,
         description="Document ID or code created by issuer",
         example="c-PCR-003",
     )
     name: str | None = pyd.Field(
         max_length=200,
+        default=None,
         description="Full document name as listed in source document",
         example="c-PCR-003 Concrete and concrete elements (EN 16757)",
     )
     short_name: str | None = pyd.Field(
         max_length=40,
+        default=None,
         description="A shortened name without boilerplate text.",
         example="Concrete and Concrete Elements",
     )
-    version: pyd.PositiveInt = pyd.Field(
+    version: str | None = pyd.Field(
         description="Document version, as expressed in document.",
         example="1.0.2",
+        default=None,
     )
     date_of_issue: datetime.date | None = pyd.Field(
         example=datetime.date(day=11, month=2, year=2022),
+        default=None,
         description="First day on which the document is valid",
     )
     valid_until: datetime.date | None = pyd.Field(
         example=datetime.date(day=11, month=2, year=2024),
+        default=None,
         description="Last day on which the document is valid",
     )
     parent: Optional["Pcr"] = pyd.Field(
         description="The parent PCR, base PCR, `Part A` PCR",
         default=None,
     )
-    # TODO: why plural?
     product_classes: dict[str, str | list[str]] = pyd.Field(
         description="List of classifications, including Masterformat and UNSPC", default_factory=dict
     )
+
+    @classmethod
+    def get_asset_type(cls) -> str | None:
+        """Return the asset type of this class (see BaseOpenEpdSchema.get_asset_type for details)."""
+        return "pcr"
```

### Comparing `openepd-0.9.0/src/openepd/model/specs/__init__.py` & `openepd-1.0.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.9.0/src/openepd/model/standard.py` & `openepd-1.0.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

