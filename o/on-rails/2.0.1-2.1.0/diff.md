# Comparing `tmp/on_rails-2.0.1.tar.gz` & `tmp/on_rails-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "on_rails-2.0.1.tar", max compression
+gzip compressed data, was "on_rails-2.1.0.tar", max compression
```

## Comparing `on_rails-2.0.1.tar` & `on_rails-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-07 10:15:49.797552 on_rails-2.0.1/LICENSE
--rw-r--r--   0        0        0    14163 2023-04-07 10:15:49.797552 on_rails-2.0.1/README.md
--rw-r--r--   0        0        0    12218 2023-04-07 10:15:49.797552 on_rails-2.0.1/on_rails/Result.py
--rw-r--r--   0        0        0     2781 2023-04-07 10:15:49.797552 on_rails-2.0.1/on_rails/ResultDetail.py
--rw-r--r--   0        0        0     1504 2023-04-07 10:15:49.797552 on_rails-2.0.1/on_rails/ResultDetails/ErrorDetail.py
--rw-r--r--   0        0        0      808 2023-04-07 10:15:49.797552 on_rails-2.0.1/on_rails/ResultDetails/Errors/BadRequestError.py
--rw-r--r--   0        0        0      819 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/ConflictError.py
--rw-r--r--   0        0        0      840 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/ExceptionError.py
--rw-r--r--   0        0        0      728 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/ForbiddenError.py
--rw-r--r--   0        0        0      726 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/InternalError.py
--rw-r--r--   0        0        0     1227 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/NotFoundError.py
--rw-r--r--   0        0        0      880 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/UnauthorizedError.py
--rw-r--r--   0        0        0      753 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/ValidationError.py
--rw-r--r--   0        0        0      474 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Errors/__init__.py
--rw-r--r--   0        0        0      573 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Success/CreatedDetail.py
--rw-r--r--   0        0        0      629 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Success/NotModifiedDetail.py
--rw-r--r--   0        0        0      831 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Success/PartialContentDetail.py
--rw-r--r--   0        0        0      188 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/Success/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/SuccessDetail.py
--rw-r--r--   0        0        0      100 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/ResultDetails/__init__.py
--rw-r--r--   0        0        0       99 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/__init__.py
--rw-r--r--   0        0        0     3337 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/_utility.py
--rw-r--r--   0        0        0     1585 2023-04-07 10:15:49.801553 on_rails-2.0.1/on_rails/decorator.py
--rw-r--r--   0        0        0      722 2023-04-07 10:15:49.801553 on_rails-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    14790 1970-01-01 00:00:00.000000 on_rails-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-07 20:45:45.970074 on_rails-2.1.0/LICENSE
+-rw-r--r--   0        0        0    14163 2023-04-07 20:45:45.970074 on_rails-2.1.0/README.md
+-rw-r--r--   0        0        0    19087 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/Result.py
+-rw-r--r--   0        0        0     2866 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetail.py
+-rw-r--r--   0        0        0     1504 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/ErrorDetail.py
+-rw-r--r--   0        0        0      808 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/BadRequestError.py
+-rw-r--r--   0        0        0      819 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ConflictError.py
+-rw-r--r--   0        0        0      840 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ExceptionError.py
+-rw-r--r--   0        0        0      728 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py
+-rw-r--r--   0        0        0      726 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/InternalError.py
+-rw-r--r--   0        0        0     1227 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/NotFoundError.py
+-rw-r--r--   0        0        0      880 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py
+-rw-r--r--   0        0        0      753 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/ValidationError.py
+-rw-r--r--   0        0        0      474 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Errors/__init__.py
+-rw-r--r--   0        0        0      573 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/CreatedDetail.py
+-rw-r--r--   0        0        0      629 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py
+-rw-r--r--   0        0        0      831 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py
+-rw-r--r--   0        0        0      188 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/Success/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/SuccessDetail.py
+-rw-r--r--   0        0        0      100 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/ResultDetails/__init__.py
+-rw-r--r--   0        0        0       99 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/__init__.py
+-rw-r--r--   0        0        0     3337 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/_utility.py
+-rw-r--r--   0        0        0     1585 2023-04-07 20:45:45.970074 on_rails-2.1.0/on_rails/decorator.py
+-rw-r--r--   0        0        0      722 2023-04-07 20:45:45.970074 on_rails-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14790 1970-01-01 00:00:00.000000 on_rails-2.1.0/PKG-INFO
```

### Comparing `on_rails-2.0.1/LICENSE` & `on_rails-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/README.md` & `on_rails-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/Result.py` & `on_rails-2.1.0/on_rails/Result.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Optional
 
 from on_rails._utility import (await_func, generate_error,
                                get_num_of_function_parameters)
 from on_rails.ResultDetail import ResultDetail
 from on_rails.ResultDetails.ErrorDetail import ErrorDetail
+from on_rails.ResultDetails.SuccessDetail import SuccessDetail
 
 
 class Result:
     """ Stores the result of a function.
 
     Attributes:
         success (bool): A flag indicating whether the result was successful.
@@ -19,14 +20,24 @@
     value: Optional[Any] = None
 
     def __init__(self, success: bool, detail: Optional[ResultDetail] = None, value: Optional[Any] = None):
         self.success = success
         self.detail = detail
         self.value = value
 
+    def __str__(self) -> str:
+        result = f"success: {self.success}\n"
+        if self.value:
+            result += f"Value: {self.value}\n"
+        if self.detail:
+            result += f"Detail:\n{self.detail}\n"
+        return result
+
+    # region Static Methods
+
     @staticmethod
     def ok(value: Optional[Any] = None, detail: Optional[ResultDetail] = None):
         """
         Returns a successful result.
 
         :param value: The value to return if the result is ok
         :type value: Optional[Any]
@@ -43,14 +54,38 @@
 
         :param detail: Optional[ResultDetail] = None
         :type detail: Optional[ResultDetail]
         :return: A failed Result object. The detail is optional.
         """
         return Result(False, detail)
 
+    @staticmethod
+    def convert_to_result(output: Any, none_means_success: bool = True):
+        """
+        The function converts a given output to a Result object, where None can indicate success or failure depending on the
+        value of a boolean parameter.
+
+        :param output: The output parameter is of type Any, which means it can be any Python object
+        :type output: Any
+        :param none_means_success: A boolean parameter that determines whether a `None` output should be considered a
+        success or a failure. If `none_means_success` is `True`, then a `None` output will be considered a success and the
+        function will return a `Result.ok()` instance. If `none_means_success` is, defaults to True
+        :type none_means_success: bool (optional)
+        :return: The function `convert_to_result` returns a `Result` object. If the `output` parameter is `None`, it returns
+        a `Result` object with a success status if `none_means_success` is `True`, otherwise it returns a `Result` object
+        with a failure status. If the `output` parameter is already a `Result` object, it returns it as is. Otherwise,
+        """
+        if output is None:
+            return Result.ok() if none_means_success else Result.fail()
+        if isinstance(output, Result):
+            return output
+        return Result.ok(output)
+
+    # endregion
+
     def code(self, default_success_code: int = 200, default_error_code: int = 500) -> int:
         """
         If the detail has a code, return that, otherwise return the default success code if the status is successful,
         otherwise return the default error code
 
         :param default_success_code: The default status code to return if the Result is successful, defaults to 200
         :type default_success_code: int (optional)
@@ -58,21 +93,15 @@
         :type default_error_code: int (optional)
         :return: int
         """
         if self.detail and self.detail.code:
             return self.detail.code
         return default_success_code if self.success else default_error_code
 
-    def __str__(self) -> str:
-        result = f"success: {self.success}\n"
-        if self.value:
-            result += f"Value: {self.value}\n"
-        if self.detail:
-            result += f"Detail:\n{self.detail}\n"
-        return result
+    # region on_success
 
     def on_success(self, func: callable, num_of_try: int = 1, try_only_on_exceptions=True):
         """
         This function executes a given function only if the previous attempts were successful.
 
         :param func: func is a function that will be executed if the previous operation was successful.
         :param num_of_try: num_of_try is an optional parameter that specifies the number of times the function should be
@@ -86,14 +115,69 @@
 
         :return: The method `on_success` returns either self or the result of given function.
         """
         if not self.success:
             return self
         return self.try_func(func, num_of_try, try_only_on_exceptions)
 
+    def on_success_add_more_data(self, more_data: object):
+        """
+        This function adds more data to the success detail if the current result is successful.
+
+        :param more_data: more_data is an object that contains additional data to be added to the success response
+        :type more_data: object
+        :return: either `ok` or `fail` result, depending on the success of adding more data to the `SuccessDetail` object.
+        """
+        if not self.success or not more_data:
+            return self
+        if not self.detail:
+            self.detail = SuccessDetail()
+        result = try_func(lambda: self.detail.add_more_data(more_data))
+        return self if result.success else result
+
+    def on_success_new_detail(self, new_detail: SuccessDetail):
+        """
+        This function updates the result detail with the new detail.
+
+        :param new_detail: new_detail is a parameter of type SuccessDetail that represents the new detail information to be
+        replaced to the current object
+        :type new_detail: SuccessDetail
+        :return: Returns result with new detail
+        """
+        if not self.success:
+            return self
+        self.detail = new_detail
+        return self
+
+    def on_success_tee(self, func: callable, num_of_try: int = 1, try_only_on_exceptions=True):
+        """
+        This function executes a given function only if the previous operation was successful and returns the original
+        object. the function result will be ignored.
+
+        :param func: func is a callable object, which means it is a function or a method that can be called. It is the
+        function that will be executed if the previous operation was successful
+        :type func: callable
+        :param num_of_try: The parameter `num_of_try` is an integer that specifies the number of times the `func` should be
+        tried in case of failure. If `num_of_try` is not specified, it defaults to 1
+        :type num_of_try: int (optional)
+        :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
+        exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
+        function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
+        :type try_only_on_exceptions: bool (optional)
+        :return: an instance of the class that it belongs to (presumably named `self`).
+        """
+        if not self.success or func is None:
+            return self
+        try_func(func, num_of_try, try_only_on_exceptions)  # ignore result
+        return self
+
+    # endregion
+
+    # region on_fail
+
     def on_fail(self, func: callable, num_of_try: int = 1, try_only_on_exceptions=True):
         """
         If the result is not successful, call the function with the given arguments
 
         :param func: The function to call
 
         :param num_of_try: num_of_try is an optional parameter that specifies the number of times the function should be
@@ -105,15 +189,95 @@
         function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
         :type try_only_on_exceptions: bool (optional)
 
         :return: The result object is being returned.
         """
         if self.success:
             return self
-        return self.try_func(func, num_of_try, ignore_previous_error=True, try_only_on_exceptions=try_only_on_exceptions)
+        return self.try_func(func, num_of_try, ignore_previous_error=True,
+                             try_only_on_exceptions=try_only_on_exceptions)
+
+    def on_fail_add_more_data(self, more_data: object, ignore_error: bool = False):
+        """
+        This function adds more data to an error detail object and returns the object
+
+        :param more_data: The parameter `more_data` is an object that contains additional data to be added to the error
+        detail.
+        :type more_data: object
+        :param ignore_error: `ignore_error` is a boolean parameter that determines whether or not to ignore any errors that
+        occur while adding more data to the `ErrorDetail` object. If `ignore_error` is set to `True`, any errors that occur
+        will be ignored and the function will continue to execute.
+        :type ignore_error: bool (optional)
+        :return: an instance of the class that it belongs to.
+        """
+        if self.success or not more_data:
+            return self
+        if not self.detail:
+            self.detail = ErrorDetail()
+        result = try_func(lambda: self.detail.add_more_data(more_data))
+        if result.success or ignore_error:
+            return self
+
+        result.detail.add_more_data(f"previous error: {self.detail}")  # pragma: no cover
+        return result  # pragma: no cover
+
+    def on_fail_new_detail(self, new_detail: ErrorDetail):
+        """
+        This function updates the result detail with the new detail.
+
+        :param new_detail: new_detail is a parameter of type SuccessDetail that represents the new detail information to be
+        replaced to the current object
+        :type new_detail: ErrorDetail
+        :return: Returns result with new detail
+        """
+        if self.success:
+            return self
+        self.detail = new_detail
+        return self
+
+    def on_fail_tee(self, func: callable, num_of_try: int = 1, try_only_on_exceptions=True):
+        """
+        This function executes a given function only if the previous operation was not successful and returns the original
+        object. the function result will be ignored.
+
+        :param func: func is a callable object, which means it is a function or a method that can be called. It is the
+        function that will be executed if the previous operation was not successful
+        :type func: callable
+        :param num_of_try: The parameter `num_of_try` is an integer that specifies the number of times the `func` should be
+        tried in case of failure. If `num_of_try` is not specified, it defaults to 1
+        :type num_of_try: int (optional)
+        :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
+        exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
+        function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
+        :type try_only_on_exceptions: bool (optional)
+        :return: an instance of the class that it belongs to (presumably named `self`).
+        """
+        if self.success or func is None:
+            return self
+        try_func(func, num_of_try, try_only_on_exceptions)  # ignore result
+        return self
+
+    def on_fail_raise_exception(self, exception_type: Optional[type] = None):
+        """
+        Request to raise the exception when the previous function failed.
+
+        :param exception_type: The `exception_type` parameter is an optional argument that specifies the type of exception
+        to be raised if the previous function fails. If this parameter is not provided, a generic `Exception` will be raised.
+        If it is provided, the specified exception type will be raised.
+        :type exception_type: Optional[type]
+        :return: Returns self or raise Exception
+        """
+        if self.success:
+            return self
+        detail = self.detail if self.detail else ""
+        if exception_type:
+            raise exception_type(str(detail))
+        raise Exception(str(detail))
+
+    # endregion
 
     def fail_when(self, condition: bool, error_detail: Optional[ErrorDetail] = None, add_prev_detail: bool = False):
         """
         If the condition is true, return a failure result with the given error detail
 
         :param condition: The condition to check. If it's True, the Result will be a failure
         :type condition: bool
@@ -123,40 +287,18 @@
         :type add_prev_detail: bool (optional)
         :return: Result object
         """
         if not condition:
             return self
 
         error_detail = error_detail if error_detail else ErrorDetail()
-        if add_prev_detail:
+        if add_prev_detail and self.detail:
             error_detail.add_more_data({"prev_detail": self.detail})
         return Result.fail(error_detail)
 
-    @staticmethod
-    def convert_to_result(output: Any, none_means_success: bool = True):
-        """
-        The function converts a given output to a Result object, where None can indicate success or failure depending on the
-        value of a boolean parameter.
-
-        :param output: The output parameter is of type Any, which means it can be any Python object
-        :type output: Any
-        :param none_means_success: A boolean parameter that determines whether a `None` output should be considered a
-        success or a failure. If `none_means_success` is `True`, then a `None` output will be considered a success and the
-        function will return a `Result.ok()` instance. If `none_means_success` is, defaults to True
-        :type none_means_success: bool (optional)
-        :return: The function `convert_to_result` returns a `Result` object. If the `output` parameter is `None`, it returns
-        a `Result` object with a success status if `none_means_success` is `True`, otherwise it returns a `Result` object
-        with a failure status. If the `output` parameter is already a `Result` object, it returns it as is. Otherwise,
-        """
-        if output is None:
-            return Result.ok() if none_means_success else Result.fail()
-        if isinstance(output, Result):
-            return output
-        return Result.ok(output)
-
     def try_func(self, func: callable, num_of_try: int = 1,
                  ignore_previous_error: bool = False, try_only_on_exceptions: bool = True):
         """
         The function `try_func` attempts to execute a given function with a specified number of tries and handles errors.
 
         :param func: `func` is a function object that will be executed by the `try_func` method. It is the main parameter of
         the method and must be provided for the method to work
```

### Comparing `on_rails-2.0.1/on_rails/ResultDetail.py` & `on_rails-2.1.0/on_rails/ResultDetail.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         if title is None or title == '':
             raise ValueError("title is required")
         self.title = title
         self.message = message
         self.code = code
         if more_data is not None:
             self.more_data = more_data
+        else:
+            self.more_data = []
 
     def is_instance_of(self, cls):
         """
         The isinstance() function is used to determine whether an object is an instance of a class or a subclass
 
         :param cls: The class to check against
         :return: True or False
@@ -56,15 +58,16 @@
 
         :param data: The data to be added to the list
         :type data: Any
         :return: None.
         """
         if data is None:
             return
-        self.more_data = []
+        if self.more_data is None:
+            self.more_data = []
         self.more_data.append(data)
 
     def __str__(self):
         """
         The function returns a string that contains the title, message, and code of the exception
         :return: str
         """
```

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/ErrorDetail.py` & `on_rails-2.1.0/on_rails/ResultDetails/ErrorDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/BadRequestError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/BadRequestError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/ConflictError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/ConflictError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/ExceptionError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/ExceptionError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/ForbiddenError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/InternalError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/InternalError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/NotFoundError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/NotFoundError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/UnauthorizedError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Errors/ValidationError.py` & `on_rails-2.1.0/on_rails/ResultDetails/Errors/ValidationError.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Success/CreatedDetail.py` & `on_rails-2.1.0/on_rails/ResultDetails/Success/CreatedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Success/NotModifiedDetail.py` & `on_rails-2.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/Success/PartialContentDetail.py` & `on_rails-2.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/ResultDetails/SuccessDetail.py` & `on_rails-2.1.0/on_rails/ResultDetails/SuccessDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/_utility.py` & `on_rails-2.1.0/on_rails/_utility.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/on_rails/decorator.py` & `on_rails-2.1.0/on_rails/decorator.py`

 * *Files identical despite different names*

### Comparing `on_rails-2.0.1/pyproject.toml` & `on_rails-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "on_rails"
-version = "2.0.1"
+version = "2.1.0"
 description = "Simple and powerful Railway Oriented library for python"
 authors = ["Payadel <payadelteam@gmail.com>"]
 readme = "README.md"
 license = "GPLV3"
 repository = "https://github.com/Payadel/on_rails"
 keywords = ["railway oriented","functional programming", "error handling"]
 packages = [{ include = "on_rails" }]
```

### Comparing `on_rails-2.0.1/PKG-INFO` & `on_rails-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: on-rails
-Version: 2.0.1
+Version: 2.1.0
 Summary: Simple and powerful Railway Oriented library for python
 Home-page: https://github.com/Payadel/on_rails
 License: GPLV3
 Keywords: railway oriented,functional programming,error handling
 Author: Payadel
 Author-email: payadelteam@gmail.com
 Requires-Python: >=3.10,<4.0
```

