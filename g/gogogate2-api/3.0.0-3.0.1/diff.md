# Comparing `tmp/gogogate2_api-3.0.0.tar.gz` & `tmp/gogogate2_api-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogogate2_api-3.0.0.tar", last modified: Wed Dec 16 16:39:00 2020, max compression
+gzip compressed data, was "gogogate2_api-3.0.1.tar", max compression
```

## Comparing `gogogate2_api-3.0.0.tar` & `gogogate2_api-3.0.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1083 2020-12-16 16:38:00.414112 gogogate2_api-3.0.0/LICENSE
--rw-r--r--   0        0        0     2372 2020-12-16 16:38:00.414112 gogogate2_api-3.0.0/README.md
--rw-r--r--   0        0        0    18078 2020-12-16 16:38:00.414112 gogogate2_api-3.0.0/gogogate2_api/__init__.py
--rwxr-xr-x   0        0        0     3958 2020-12-16 16:38:00.414112 gogogate2_api-3.0.0/gogogate2_api/cli.py
--rw-r--r--   0        0        0    16874 2020-12-16 16:38:00.414112 gogogate2_api-3.0.0/gogogate2_api/common.py
--rw-r--r--   0        0        0      800 2020-12-16 16:38:00.414112 gogogate2_api-3.0.0/gogogate2_api/const.py
--rw-r--r--   0        0        0     3172 2020-12-16 16:38:00.414112 gogogate2_api-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3600 2020-12-16 16:39:00.893869 gogogate2_api-3.0.0/setup.py
--rw-r--r--   0        0        0     3402 2020-12-16 16:39:00.894403 gogogate2_api-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-24 15:55:40.793650 gogogate2_api-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2414 2023-06-24 15:55:40.793650 gogogate2_api-3.0.1/README.md
+-rw-r--r--   0        0        0    18116 2023-06-24 15:55:40.793650 gogogate2_api-3.0.1/gogogate2_api/__init__.py
+-rwxr-xr-x   0        0        0     3974 2023-06-24 15:55:40.793650 gogogate2_api-3.0.1/gogogate2_api/cli.py
+-rw-r--r--   0        0        0    17022 2023-06-24 15:55:40.797650 gogogate2_api-3.0.1/gogogate2_api/common.py
+-rw-r--r--   0        0        0      801 2023-06-24 15:55:40.797650 gogogate2_api-3.0.1/gogogate2_api/const.py
+-rw-r--r--   0        0        0     3513 2023-06-24 15:55:40.797650 gogogate2_api-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 gogogate2_api-3.0.1/PKG-INFO
```

### Comparing `gogogate2_api-3.0.0/LICENSE` & `gogogate2_api-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gogogate2_api-3.0.0/README.md` & `gogogate2_api-3.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Python gogogate2-api [![Build status](https://github.com/vangorra/python_gogogate2_api/workflows/Build/badge.svg?branch=master)](https://github.com/vangorra/python_gogogate2_api/actions?workflow=Build) [![codecov](https://codecov.io/gh/vangorra/python_gogogate2_api/branch/master/graph/badge.svg)](https://codecov.io/gh/vangorra/python_gogogate2_api) [![PyPI](https://img.shields.io/pypi/v/gogogate2-api)](https://pypi.org/project/gogogate2-api/)
+# Python gogogate2-api [![Build status](https://github.com/vangorra/python_gogogate2_api/workflows/Build/badge.svg?branch=master)](https://github.com/vangorra/python_gogogate2_api/actions?workflow=Build) [![Coverage Status](https://coveralls.io/repos/github/vangorra/python_gogogate2_api/badge.svg?branch=devops_cleanup)](https://coveralls.io/github/vangorra/python_gogogate2_api?branch=master) [![PyPI](https://img.shields.io/pypi/v/gogogate2-api)](https://pypi.org/project/gogogate2-api/)
 Python library for controlling GogoGate2 and iSmartGate devices
 
 
 ## Installation
 
     pip install gogogate2-api
```

### Comparing `gogogate2_api-3.0.0/gogogate2_api/__init__.py` & `gogogate2_api-3.0.1/gogogate2_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,28 @@
     CredentialsNotSetException,
     DoorNotSetException,
     DoorStatus,
     ExceptionGenerator,
     GogoGate2ActivateResponse,
     GogoGate2InfoResponse,
     InvalidApiCodeException,
+    InvalidDoorException,
     InvalidOptionException,
     ISmartGateActivateResponse,
     ISmartGateDoor,
     ISmartGateInfoResponse,
     RequestOption,
     TransitionDoorStatus,
     element_to_api_error,
     element_to_gogogate2_activate_response,
     element_to_gogogate2_info_response,
     element_to_ismartgate_activate_response,
     element_to_ismartgate_info_response,
     get_configured_doors,
     get_door_by_id,
-    InvalidDoorException,
 )
 from .const import GogoGate2ApiErrorCode, ISmartGateApiErrorCode
 
 
 class ApiCipher:
     """AES/CBC/PKCS5Padding algorithm."""
 
@@ -107,17 +107,17 @@
 
     def __init__(self, username: str, password: str) -> None:
         """Initialize the object."""
         self._username: Final = username
         self._password: Final = password
 
         # Calculate the token.
-        raw_token: Final[
-            str
-        ] = ISmartGateApiCipher.RAW_TOKEN_FORMAT % self._username.lower()
+        raw_token: Final[str] = (
+            ISmartGateApiCipher.RAW_TOKEN_FORMAT % self._username.lower()
+        )
         self._token: Final = sha1(raw_token.encode("utf-8")).hexdigest()  # nosec
 
         # Calculate the key and pass it onto the superclass.
         sha1_hex_str: Final = sha1(  # nosec
             (self._username.lower() + self._password).encode()
         ).hexdigest()
 
@@ -127,42 +127,42 @@
 
     @property
     def token(self) -> str:
         """Get the token."""
         return self._token
 
 
-ApiCipherType = TypeVar(
-    "ApiCipherType", bound=Union[GogoGate2ApiCipher, ISmartGateApiCipher]
+ApiCipherTypeVar = TypeVar(
+    "ApiCipherTypeVar", bound=Union[GogoGate2ApiCipher, ISmartGateApiCipher]
 )
-InfoResponseType = TypeVar(
-    "InfoResponseType", bound=Union[GogoGate2InfoResponse, ISmartGateInfoResponse]
+InfoResponseTypeVar = TypeVar(
+    "InfoResponseTypeVar", bound=Union[GogoGate2InfoResponse, ISmartGateInfoResponse]
 )
-ActivateResponseType = TypeVar(
-    "ActivateResponseType",
+ActivateResponseTypeVar = TypeVar(
+    "ActivateResponseTypeVar",
     bound=Union[GogoGate2ActivateResponse, ISmartGateActivateResponse],
 )
 
 
 # pylint: disable=too-many-instance-attributes
 class AbstractGateApi(
-    Generic[ApiCipherType, InfoResponseType, ActivateResponseType], abc.ABC
+    Generic[ApiCipherTypeVar, InfoResponseTypeVar, ActivateResponseTypeVar], abc.ABC
 ):
     """API capable of communicating with a gogogate2 devices."""
 
     API_URL_TEMPLATE: Final = "http://%s/api.php"
     DEFAULT_REQUEST_TIMEOUT = timedelta(seconds=20)
     DEFAULT_TRANSITION_STATUS_TIMEOUT = timedelta(seconds=55)
 
     def __init__(
         self,
         host: str,
         username: str,
         password: str,
-        api_cipher: ApiCipherType,
+        api_cipher: ApiCipherTypeVar,
         request_timeout: timedelta = DEFAULT_REQUEST_TIMEOUT,
         transition_status_timeout: timedelta = DEFAULT_TRANSITION_STATUS_TIMEOUT,
     ) -> None:
         """Initialize the object."""
         self._host: Final = host
         self._username: Final = username
         self._password: Final = password
@@ -184,15 +184,15 @@
 
     @property
     def password(self) -> str:
         """Get the password."""
         return self._password
 
     @property
-    def cipher(self) -> ApiCipherType:
+    def cipher(self) -> ApiCipherTypeVar:
         """Get the cipher."""
         return self._cipher
 
     async def _async_request(
         self,
         option: RequestOption,
         arg1: Optional[str] = None,
@@ -234,45 +234,44 @@
             raise self._get_exception_map().get(api_error.code, ApiError)(
                 api_error.code, api_error.message
             )
 
         return cast(Element, root_element)
 
     @abc.abstractmethod
-    async def async_info(self) -> InfoResponseType:
+    async def async_info(self) -> InfoResponseTypeVar:
         """Get info about the device and doors."""
 
     @abc.abstractmethod
-    async def async_activate(self, door_id: int) -> ActivateResponseType:
+    async def async_activate(self, door_id: int) -> ActivateResponseTypeVar:
         """Send a command to open/close/stop the door.
 
         Devices do not have a status for opening or closing. So running
         this method during an action will stop the door. It's recommended you
         use open_door() or close_door() as those methods check the status
         before running and run if needed."""
 
     @abc.abstractmethod
-    def _get_activate_api_code(self, info: InfoResponseType, door_id: int) -> str:
+    def _get_activate_api_code(self, info: InfoResponseTypeVar, door_id: int) -> str:
         """Get api code for activate actions."""
 
     @staticmethod
     @abc.abstractmethod
     def _get_exception_map() -> Dict[int, ExceptionGenerator]:
         """Return a more specific exception."""
 
-    # pylint: disable=no-self-use
     def _get_extra_url_params(self) -> Dict[str, str]:
         return {}
 
     async def _async_info(self) -> Element:
         """Get info about the device and doors."""
         return await self._async_request(RequestOption.INFO)
 
     async def _async_activate(
-        self, door_id: int, info: Optional[InfoResponseType] = None
+        self, door_id: int, info: Optional[InfoResponseTypeVar] = None
     ) -> Element:
         """Send a command to open/close/stop the door.
 
         Gogogate2/iSmartGate do not have a status for opening or closing. So
         running this method during an action will stop the door. It's
         recommended you use open_door() or close_door() as those methods check
         the status before running and run if needed."""
@@ -296,16 +295,24 @@
 
         # Get current door status.
         info: Final = await self.async_info()
         statuses: Final = self._get_door_statuses(
             info, use_transitional_status=consider_transitional_states
         )
         current_door_status: Final = statuses.get(door_id)
-        result_door_statuses: Final = OPEN_DOOR_STATUSES if target_door_status == DoorStatus.OPENED else CLOSE_DOOR_STATUSES
-        transitional_door_status: Final = TransitionDoorStatus.OPENING if target_door_status == DoorStatus.OPENED else TransitionDoorStatus.CLOSING
+        result_door_statuses: Final = (
+            OPEN_DOOR_STATUSES
+            if target_door_status == DoorStatus.OPENED
+            else CLOSE_DOOR_STATUSES
+        )
+        transitional_door_status: Final = (
+            TransitionDoorStatus.OPENING
+            if target_door_status == DoorStatus.OPENED
+            else TransitionDoorStatus.CLOSING
+        )
 
         # Door is invalid, not configured, already in desired state or transitioning to it.
         if not current_door_status or current_door_status in result_door_statuses:
             return False
 
         await self._async_activate(door_id, info)
 
@@ -342,22 +349,23 @@
         return await self._async_set_door_status(
             door_id,
             DoorStatus.OPENED,
             consider_transitional_states=consider_transitional_states,
         )
 
     def _get_door_statuses(
-        self, info: InfoResponseType, use_transitional_status: bool = True
+        self, info: InfoResponseTypeVar, use_transitional_status: bool = True
     ) -> Dict[int, AllDoorStatus]:
         doors: Final = get_configured_doors(info)
 
         # Clean out the cache.
-        for (cached_door_id, cached_transitional_status,) in list(
-            self._transition_door_status.items()
-        ):
+        for (
+            cached_door_id,
+            cached_transitional_status,
+        ) in list(self._transition_door_status.items()):
             if (
                 datetime.utcnow() - cached_transitional_status.activated
                 >= self._transition_status_timeout
             ):
                 del self._transition_door_status[cached_door_id]
 
         # For each door, determine the status.
@@ -420,15 +428,14 @@
         this method during an action will stop the door. It's recommended you
         use open_door() or close_door() as those methods check the status
         before running and run if needed."""
         return element_to_ismartgate_activate_response(
             await self._async_activate(door_id)
         )
 
-    #  pylint: disable=no-self-use
     def _get_activate_api_code(self, info: ISmartGateInfoResponse, door_id: int) -> str:
         """Get api code for activate actions."""
         door: Final = get_door_by_id(door_id, info)
         if not door:
             raise InvalidDoorException(door_id)
 
         return cast(ISmartGateDoor, door).apicode
@@ -499,11 +506,10 @@
             GogoGate2ApiErrorCode.CREDENTIALS_NOT_SET.value: CredentialsNotSetException,
             GogoGate2ApiErrorCode.CREDENTIALS_INCORRECT.value: CredentialsIncorrectException,
             GogoGate2ApiErrorCode.INVALID_OPTION.value: InvalidOptionException,
             GogoGate2ApiErrorCode.INVALID_API_CODE.value: InvalidApiCodeException,
             GogoGate2ApiErrorCode.DOOR_NOT_SET.value: DoorNotSetException,
         }
 
-    # pylint: disable=unused-argument, no-self-use
     def _get_activate_api_code(self, info: GogoGate2InfoResponse, door_id: int) -> str:
         """Get api code for activate actions."""
         return info.apicode
```

### Comparing `gogogate2_api-3.0.0/gogogate2_api/cli.py` & `gogogate2_api-3.0.1/gogogate2_api/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,19 @@
     required=True,
     type=click.Choice([item.value for item in DeviceType], case_sensitive=False),
     hidden=True,
 )
 @click.version_option()
 @click.pass_context
 def cli(
-    ctx: click.core.Context, host: str, username: str, password: str, device_type: str,
+    ctx: click.core.Context,
+    host: str,
+    username: str,
+    password: str,
+    device_type: str,
 ) -> None:
     """Interact with the device API."""
     api_generator: Callable[[str, str, str], Union[GogoGate2Api, ISmartGateApi]]
 
     if device_type == DeviceType.GOGOGATE2.value:
         api_generator = GogoGate2Api
     else:
```

### Comparing `gogogate2_api-3.0.0/gogogate2_api/common.py` & `gogogate2_api-3.0.1/gogogate2_api/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Callable, Optional, Tuple, Type, TypeVar, Union, cast
 from xml.etree.ElementTree import Element  # nosec
 
 from typing_extensions import Final
 
 from .const import NONE_INT
 
-GenericType = TypeVar("GenericType")
+GenericTypeVar = TypeVar("GenericTypeVar")
 
 
 class InvalidDoorException(Exception):
     """Exception when door is invalid."""
 
     def __init__(self, door_id: int) -> None:
         super().__init__(f"Door with id {door_id} not found.")
@@ -23,20 +23,15 @@
 
 
 class TagException(Exception):
     """General exception for tags."""
 
     def __init__(self, tag: str, message: str) -> None:
         super().__init__(message)
-        self._tag: Final = tag
-
-    @property
-    def tag(self) -> str:
-        """Get the tag."""
-        return self._tag
+        self.tag: Final = tag
 
 
 class TagNotFoundException(TagException):
     """Thrown when encountering an unexpected type."""
 
     def __init__(self, tag: str) -> None:
         """Initialize."""
@@ -50,44 +45,34 @@
         """Initialize."""
         super().__init__(tag, f"Text was empty for tag '{tag}'.")
 
 
 class UnexpectedTypeException(Exception):
     """Thrown when encountering an unexpected type."""
 
-    def __init__(self, value: Any, expected: Type[GenericType]):
+    def __init__(self, value: Any, expected: Type[GenericTypeVar]):
         """Initialize."""
         super().__init__(
-            'Expected of "%s" to be "%s" but was "%s."' % (value, expected, type(value))
+            f'Expected of "{value}" to be "{expected}" but was "{type(value)}."'
         )
-        self._value: Final = value
-        self._expected: Final = expected
+        self.value: Final = value
+        self.expected: Final = expected
 
-    @property
-    def value(self) -> Any:
-        """Get value."""
-        return self._value
 
-    @property
-    def expected(self) -> Type[GenericType]:
-        """Get expected type."""
-        return self._expected
-
-
-def enforce_type(value: Any, expected: Type[GenericType]) -> GenericType:
+def enforce_type(value: Any, expected: Type[GenericTypeVar]) -> GenericTypeVar:
     """Enforce a data type."""
     if not isinstance(value, expected):
         raise UnexpectedTypeException(value, expected)
 
     return value
 
 
 def value_or_none(
-    value: Any, convert_fn: Callable[[Any], GenericType]
-) -> Union[GenericType, None]:
+    value: Any, convert_fn: Callable[[Any], GenericTypeVar]
+) -> Union[GenericTypeVar, None]:
     """Convert a value given a specific conversion function."""
     if value is None:
         return None
 
     try:
         return convert_fn(value)
     except Exception:  # pylint: disable=broad-except
@@ -175,15 +160,15 @@
     """Invalid api code exception."""
 
 
 class DoorNotSetException(ApiError):
     """Door not set exception."""
 
 
-ExceptionGenerator: Final = Callable[[int, str], ApiError]
+ExceptionGenerator = Callable[[int, str], ApiError]
 
 
 class DoorStatus(Enum):
     """Door status."""
 
     CLOSED = "closed"
     OPENED = "opened"
@@ -193,15 +178,15 @@
 class TransitionDoorStatus(Enum):
     """Presumed door status."""
 
     OPENING = "opening"
     CLOSING = "closing"
 
 
-AllDoorStatus: Final = Union[DoorStatus, TransitionDoorStatus]
+AllDoorStatus = Union[DoorStatus, TransitionDoorStatus]
 
 
 CLOSE_DOOR_STATUSES: Final = frozenset(
     (DoorStatus.CLOSED, TransitionDoorStatus.CLOSING)
 )
 OPEN_DOOR_STATUSES: Final = frozenset((DoorStatus.OPENED, TransitionDoorStatus.OPENING))
 
@@ -363,14 +348,28 @@
     found_element: Final = element_or_none(element, tag)
     if found_element is None:
         raise TagNotFoundException(tag)
 
     return found_element
 
 
+def element_text_or_empty(element: Optional[Element], tag: str) -> str:
+    """Get element value as text or an empty string."""
+    return element_text_or_default(element, tag, "")
+
+
+def element_text_or_default(element: Optional[Element], tag: str, default: str) -> str:
+    """Get element value as text or a default value."""
+    val: Final = element_text_or_none(element, tag)
+    if val is None:
+        return default
+
+    return cast(str, val)
+
+
 def element_text_or_none(element: Optional[Element], tag: str) -> Optional[str]:
     """Get element text from xml element."""
     found_element: Final = element_or_none(element, tag)
     return (
         None
         if found_element is None
         else None
@@ -412,15 +411,17 @@
         linkquality=element_text_or_none(element, "linkquality"),
         signal=element_text_or_none(element, "signal"),
     )
 
 
 def network_or_raise(element: Element) -> Network:
     """Get network from xml element."""
-    return Network(ip=element_text_or_raise(element, "ip"),)
+    return Network(
+        ip=element_text_or_raise(element, "ip"),
+    )
 
 
 def outputs_or_raise(element: Element) -> Outputs:
     """Get outputs from xml element."""
     return Outputs(
         output1=element_text_or_raise(element, "output1").lower() == "on",
         output2=element_text_or_raise(element, "output2").lower() == "on",
@@ -455,17 +456,17 @@
 
 def ismartgate_door_or_raise(door_id: int, element: Element) -> ISmartGateDoor:
     """Get door from xml element."""
     temp: Final = float_or_none(element_text_or_none(element, "temperature"))
     voltage: Final = int_or_none(element_text_or_none(element, "voltage"))
     return ISmartGateDoor(
         door_id=door_id,
-        enabled=element_text_or_raise(element, "enabled").lower() == "yes",
-        apicode=element_text_or_raise(element, "apicode"),
-        customimage=element_text_or_raise(element, "customimage").lower() == "yes",
+        enabled=element_text_or_empty(element, "enabled").lower() == "yes",
+        apicode=element_text_or_empty(element, "apicode"),
+        customimage=element_text_or_empty(element, "customimage").lower() == "yes",
         permission=element_text_or_raise(element, "permission").lower() == "yes",
         name=element_text_or_none(element, "name"),
         gate=element_text_or_raise(element, "gate").lower() == "yes",
         mode=cast(
             DoorMode, enum_or_raise(element_text_or_raise(element, "mode"), DoorMode)
         ),
         status=cast(
@@ -568,8 +569,8 @@
         ),
         None,
     )
 
 
 def get_configured_doors(response: AbstractInfoResponse) -> Tuple[AbstractDoor, ...]:
     """Get a tuple of configured doors from a response."""
-    return tuple([door for door in get_doors(response) if door.name])
+    return tuple(door for door in get_doors(response) if door.name)
```

### Comparing `gogogate2_api-3.0.0/gogogate2_api/const.py` & `gogogate2_api-3.0.1/gogogate2_api/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Constants for gate devices"""
 from enum import IntEnum
+
 from typing_extensions import Final
 
 
 class GogoGate2ApiErrorCode(IntEnum):
     """Common API error codes."""
 
     CREDENTIALS_NOT_SET = 2
```

### Comparing `gogogate2_api-3.0.0/pyproject.toml` & `gogogate2_api-3.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gogogate2_api"
-version = "3.0.0"
+version = "3.0.1"
 description = "Library for connecting to GogoGate2 and iSmartGate hubs"
 
 license = "MIT"
 
 authors = [
     "Robbie Van Gorkom <robbie.van.gorkom@protonmail.com>"
 ]
@@ -17,46 +17,44 @@
 keywords = ['gogogate2', 'ismartgate', 'api']
 
 [tool.poetry.scripts]
 gogogate2 = "gogogate2_api.cli:gogogate2_cli"
 ismartgate = "gogogate2_api.cli:ismartgate_cli"
 
 [tool.poetry.dependencies]
-python = ">=3.6, <4"
-dataclasses = { version = "^0.7", python = "^3.6, <3.7" }
+python = ">=3.8.1, <4"
 defusedxml = ">=0.6.0"
 pycryptodome = ">=3.9.7"
 requests = ">=2.23.0"
 typing-extensions = ">=3.7.4.2"
-httpx = "^0.16.1"
+httpx = ">=0.16.1"
+click = ">=7.1.2"
 
 [tool.poetry.dev-dependencies]
-autoflake = "==1.3.1"
-bandit = "==1.6.2"
-black = "==19.10b0"
-click = "==7.1.2"
-codespell = "==1.17.1"
-coverage = "==5.0.4"
-dicttoxml = "==1.7.4"
-flake8 = "==3.7.8"
-isort = "==4.3.21"
-mypy = "==0.740"
-pylint = "==2.5.3"
-pytest = "==6.0.1"
-pytest-cov = "==2.10.0"
-responses = "==0.10.6"
-toml = "==0.10.0"  # Needed by isort and others to parse this file.
-wheel = "==0.33.6"  # Needed for successful compile of other modules.
-respx = "^0.16.3"
-pytest-asyncio = "^0.14.0"
+autoflake = "==2.1.1"
+bandit = "==1.7.5"
+black = "==23.3.0"
+codespell = "==2.2.5"
+coverage = "==7.2.7"
+dicttoxml2 = "==2.1.0"
+flake8 = "==6.0.0"
+isort = "==5.12.0"
+mypy = "==1.4.0"
+pylint = "==2.17.4"
+pytest = "==7.4.0"
+pytest-cov = "==4.1.0"
+responses = "==0.23.1"
+toml = "==0.10.2"  # Needed by isort and others to parse this file.
+wheel = "==0.40.0"  # Needed for successful compile of other modules.
+respx = ">=0.16.3"
+pytest-asyncio = "^0.21.0"
 asynctest = "^0.13.0"
 
-
 [tool.black]
-target-version = ["py36", "py37", "py38"]
+target-version = ["py38"]
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
     | \.mypy_cache
@@ -95,15 +93,15 @@
 combine_as_imports = true
 
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
-fail_under = 97.0
+fail_under = 98.0
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--capture no --cov ./gogogate2_api --cov-report html:build/coverage_report --cov-report term --cov-report xml:build/coverage.xml"
 
 
 [tool.pylint.MASTER]
@@ -127,8 +125,29 @@
 # For attrs
 ignored-classes="responses"
 
 [tool.pylint.FORMAT]
 expected-line-ending-format="LF"
 
 [tool.pylint.EXCEPTIONS]
-overgeneral-exceptions="Exception"
+overgeneral-exceptions="builtin.Exception"
+
+[tool.mypy]
+ignore_missing_imports = true
+follow_imports = "normal"
+follow_imports_for_stubs = true
+
+disallow_subclassing_any = true
+
+disallow_untyped_calls = true
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+check_untyped_defs = true
+
+no_implicit_optional = true
+
+warn_unused_ignores = true
+warn_return_any = true
+warn_unreachable = true
+
+implicit_reexport = true
+strict_equality = true
```

### Comparing `gogogate2_api-3.0.0/PKG-INFO` & `gogogate2_api-3.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: gogogate2-api
-Version: 3.0.0
+Version: 3.0.1
 Summary: Library for connecting to GogoGate2 and iSmartGate hubs
 Home-page: https://github.com/vangorra/python_gogogate2_api
 License: MIT
 Keywords: gogogate2,ismartgate,api
 Author: Robbie Van Gorkom
 Author-email: robbie.van.gorkom@protonmail.com
-Requires-Python: >=3.6,<4
+Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: dataclasses (>=0.7,<0.8); python_version >= "3.6" and python_version < "3.7"
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=7.1.2)
 Requires-Dist: defusedxml (>=0.6.0)
-Requires-Dist: httpx (>=0.16.1,<0.17.0)
+Requires-Dist: httpx (>=0.16.1)
 Requires-Dist: pycryptodome (>=3.9.7)
 Requires-Dist: requests (>=2.23.0)
 Requires-Dist: typing-extensions (>=3.7.4.2)
 Project-URL: Repository, https://github.com/vangorra/python_gogogate2_api
 Description-Content-Type: text/markdown
 
-# Python gogogate2-api [![Build status](https://github.com/vangorra/python_gogogate2_api/workflows/Build/badge.svg?branch=master)](https://github.com/vangorra/python_gogogate2_api/actions?workflow=Build) [![codecov](https://codecov.io/gh/vangorra/python_gogogate2_api/branch/master/graph/badge.svg)](https://codecov.io/gh/vangorra/python_gogogate2_api) [![PyPI](https://img.shields.io/pypi/v/gogogate2-api)](https://pypi.org/project/gogogate2-api/)
+# Python gogogate2-api [![Build status](https://github.com/vangorra/python_gogogate2_api/workflows/Build/badge.svg?branch=master)](https://github.com/vangorra/python_gogogate2_api/actions?workflow=Build) [![Coverage Status](https://coveralls.io/repos/github/vangorra/python_gogogate2_api/badge.svg?branch=devops_cleanup)](https://coveralls.io/github/vangorra/python_gogogate2_api?branch=master) [![PyPI](https://img.shields.io/pypi/v/gogogate2-api)](https://pypi.org/project/gogogate2-api/)
 Python library for controlling GogoGate2 and iSmartGate devices
 
 
 ## Installation
 
     pip install gogogate2-api
```

