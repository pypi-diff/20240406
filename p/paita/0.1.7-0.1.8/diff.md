# Comparing `tmp/paita-0.1.7.tar.gz` & `tmp/paita-0.1.8.tar.gz`

## Comparing `paita-0.1.7.tar` & `paita-0.1.8.tar`

### file list

```diff
@@ -1,54 +1,57 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 paita-0.1.7/mypy.ini
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 paita-0.1.7/.github/workflows/code_quality.yml
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 paita-0.1.7/docs/development.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 paita-0.1.7/docs/publish.md
--rw-r--r--   0        0        0   477378 2020-02-02 00:00:00.000000 paita-0.1.7/imgs/paita.jpg
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/__about__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/__init__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/__init__.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/bedrock.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/callbacks.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/chat.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/chat_history.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/enums.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/message.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/mock_model.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/ai/models.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/localization/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/localization/labels.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/__init__.py
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/app.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/error_screen.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/message_box.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/multi_line_input.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/settings_screen.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/wait_screen.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/styles/app.tcss
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/styles/error_screen.tcss
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/styles/message_box.tcss
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/styles/settings_screen.tcss
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/tui/styles/wait_screen.tcss
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/utils/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/utils/asyncify.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/utils/config_dirs.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/utils/logger.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/utils/settings_manager.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/utils/settings_model.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 paita-0.1.7/src/paita/utils/string_utils.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/tests/integration/__init__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/tests/integration/ai/__init__.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 paita-0.1.7/tests/integration/ai/test_chat.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 paita-0.1.7/tests/integration/ai/test_models.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/tests/unit/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 paita-0.1.7/tests/unit/test_cache3.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 paita-0.1.7/tests/unit/test_settings_manager.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 paita-0.1.7/tests/unit/test_string_utils.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.7/tests/unit/ai/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 paita-0.1.7/tests/unit/ai/test_chat.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 paita-0.1.7/tests/unit/ai/test_message.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 paita-0.1.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 paita-0.1.7/LICENSE
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 paita-0.1.7/README.md
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 paita-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 paita-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 paita-0.1.8/mypy.ini
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 paita-0.1.8/.github/workflows/code_quality.yml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 paita-0.1.8/docs/development.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 paita-0.1.8/docs/publish.md
+-rw-r--r--   0        0        0   477378 2020-02-02 00:00:00.000000 paita-0.1.8/imgs/paita.jpg
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/__about__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/__init__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/__init__.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/callbacks.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/chat.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/chat_history.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/enums.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/message.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/__init__.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/bedrock.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/mock.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/ollama.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/openai.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/service.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/localization/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/localization/labels.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/__init__.py
+-rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/app.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/error_screen.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/message_box.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/multi_line_input.py
+-rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/settings_screen.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/wait_screen.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/app.tcss
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/error_screen.tcss
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/message_box.tcss
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/settings_screen.tcss
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/wait_screen.tcss
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/config_dirs.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/logger.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/settings_manager.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/settings_model.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/string_utils.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/__init__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/ai/__init__.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/ai/test_chat.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/ai/test_models.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/test_cache3.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/test_settings_manager.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/test_string_utils.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/ai/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/ai/test_chat.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/ai/test_message.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 paita-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 paita-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 paita-0.1.8/README.md
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 paita-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 paita-0.1.8/PKG-INFO
```

### Comparing `paita-0.1.7/.github/workflows/code_quality.yml` & `paita-0.1.8/.github/workflows/code_quality.yml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         run: |
           python -m pip install hatch
       - name: Run format and lint check
         run: hatch fmt --check
 #      - name: Run mypy
 #        run: hatch run mypy src tests
       - name: Run Tests
-        run: hatch run +py=${{ matrix.python-version }} test:cov
+        run: hatch run +py=${{ matrix.python-version }} test:github-cov
       - name: Disambiguate coverage filename
         run: mv .coverage ".coverage.${{ matrix.os }}.${{ matrix.python-version }}"
       - name: Upload coverage data
         uses: actions/upload-artifact@v4
         with:
           name: coverage-${{ matrix.os }}-${{ matrix.python-version }}
           path: .coverage*
```

### Comparing `paita-0.1.7/docs/development.md` & `paita-0.1.8/docs/development.md`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/docs/publish.md` & `paita-0.1.8/docs/publish.md`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/imgs/paita.jpg` & `paita-0.1.8/imgs/paita.jpg`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/ai/callbacks.py` & `paita-0.1.8/src/paita/ai/callbacks.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/ai/chat_history.py` & `paita-0.1.8/src/paita/ai/chat_history.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/ai/mock_model.py` & `paita-0.1.8/src/paita/ai/services/mock.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/tui/app.py` & `paita-0.1.8/src/paita/tui/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,16 +58,15 @@
         self._current_message: Union[MessageBox or None] = None
         self._current_id: str = "id_0"
         self._last_focused: Union[Widget or None] = None
 
         self._chat_history = ChatHistory(app_name=label.APP_TITLE, app_author=label.APP_AUTHOR)
 
     def compose(self) -> ComposeResult:
-        log.debug("compose")
-        yield Header()  # show_clock=True)
+        yield Header(show_clock=True)
         with Container(id="body"):
             vertical_scroll: VerticalScroll = VerticalScroll(id="conversation")
             vertical_scroll.can_focus = False
             yield vertical_scroll
             with Horizontal(id="input_box"):
                 if TEXT_AREA:
                     yield MultiLineInput(id="multi_line_input", multiline=True)
@@ -75,54 +74,47 @@
                     yield Input(id="input")
                 yield Button(label="Send", variant="success", id="send_button")
         yield Footer()
 
     # Action handlers
 
     async def on_button_pressed(self, event: Button.Pressed) -> None:
-        log.debug("on_button_pressed")
         if event.button.id == "send_button":
             await self.process_conversation()
 
     async def on_input_submitted(self, event: Input.Submitted) -> None:
-        log.debug("on_input_submitted")
         if event.input.id in ("input", "multi_line_input"):
             await self.process_conversation()
 
     def action_settings(self, allow_cancel: bool = False) -> None:  # noqa: FBT001, FBT002
-        log.debug("action_settings")
         self.push_screen(
             SettingsScreen(
                 settings=self._settings,
                 cache=self._cache,
                 allow_cancel=allow_cancel,
             ),
             self.exit_settings,
         )
 
     async def action_clear(self) -> None:
-        log.debug("action_clear")
         await self._chat_history.history.aclear()
         await self.query_one("#conversation").remove()
         await self.query_one("#body").mount(VerticalScroll(id="conversation"))
 
     def action_quit(self) -> None:
-        log.debug("action_quit")
         self._cache.clear()
         self.exit()
 
     # Callbacks
 
     def exit_settings(self, changed: bool = False):  # noqa: FBT001, FBT002
-        log.debug("exit_settings")
         if changed:
             self.init_chat()
 
     async def on_mount(self) -> None:
-        log.debug("on_mount")
         # TODO: If history is loaded here then scroll to end works
         # however input area text doesn't work properly
         # when calling _mount_chat_history later then text input works but scroll not
         # await self._mount_chat_history()
         try:
             await self.push_screen(WaitScreen(label.APP_LIST_AI_SERVICES_MODELS))
             await self._list_models()
@@ -150,27 +142,25 @@
                 model=SettingsModel(),
                 app_name=label.APP_TITLE,
                 app_author=label.APP_AUTHOR,
             )
             self.action_settings(allow_cancel=False)
 
     def init_chat(self):
-        log.debug("init_chat")
         if self._chat is None:
             self._chat = Chat()
         callback_handler = AsyncHandler()
         callback_handler.register_callbacks(self.callback_on_token, self.callback_on_end, self.callback_on_error)
         self._chat.init_model(settings_model=self._settings.model, callback_handler=callback_handler)
         if TEXT_AREA:
             self.query_one("#multi_line_input").focus()
         else:
             self.query_one("#input").focus()
 
     async def process_conversation(self) -> None:
-        log.debug("process_conversation")
         if TEXT_AREA:
             text_input: MultiLineInput = self.query_one("#multi_line_input")
             question = text_input.text
         else:
             text_input: Input = self.query_one("#input", Input)
             question = text_input.value
 
@@ -198,31 +188,28 @@
             await self._chat.request(question, chat_history=self._chat_history)
         except ValueError as e:
             log.info(str(e))
         except Exception as e:  # noqa: BLE001
             log.exception(e)
 
     def toggle_widgets(self, *widgets: Widget) -> None:
-        log.debug("toggle_widgets")
         for w in widgets:
             w.disabled = not w.disabled
 
     def callback_on_token(self, data: str):
-        log.debug(f"callback_on_token: {data}")
         if self._current_message is None:
             loading_indication = self.query_one(LoadingIndicator)
             loading_indication.remove()
             self._current_message = MessageBox(data, role="answer")
             conversation = self.query_one("#conversation")
             conversation.mount(self._current_message)
         else:
             self._current_message.append(data)
 
     def callback_on_end(self, data: str):
-        log.debug(f"callback_on_end: {data}")
         conversation = self.query_one("#conversation")
         if self._current_message is None:
             loading_indication = self.query_one(LoadingIndicator)
             loading_indication.remove()
             self._current_message = MessageBox(data, role="answer")
             conversation.mount(self._current_message)
 
@@ -231,54 +218,52 @@
 
         text_input = self.query_one("#multi_line_input") if TEXT_AREA else self.query_one("#input")
         button = self.query_one("#send_button")
         self.toggle_widgets(text_input, button)
         text_input.focus()
 
     def callback_on_error(self, error):
-        log.debug(f"callback_on_error: {error}")
         if self._current_message:
             loading_indication = self.query_one(LoadingIndicator)
             loading_indication.remove()
             self._current_message.flush()
             self._current_message = None
 
         self.push_screen(ErrorScreen(str(error)), self.exit_error_screen)
 
-    def exit_error_screen(self, result: str):
-        log.debug(f"exit_error_screen {result}")
+    def exit_error_screen(self, exit_app: bool = False):  # noqa: FBT001, FBT002
+        if exit_app:
+            self.exit()
+
         loading_indication = self.query_one(LoadingIndicator)
         loading_indication.remove()
 
         text_input = self.query_one("#multi_line_input") if TEXT_AREA else self.query_one("#input")
         button = self.query_one("#send_button")
         self.toggle_widgets(text_input, button)
 
         text_input.focus()
 
     async def _mount_chat_history(self):
-        log.debug("_mount_chat_history")
         messages = await self._chat_history.messages()
         message_boxes: [MessageBox] = [
             MessageBox(data=message.content, role=message.role.value) for message in messages
         ]
         conversation = self.query_one("#conversation")
         await conversation.mount_all(message_boxes)
         conversation.scroll_end(animate=False)
 
     async def _list_models(self):
-        log.debug("_list_models")
         self.push_screen(WaitScreen(label.APP_LIST_AI_SERVICES_MODELS))
         all_models = await list_all_models()
         self.pop_screen()
         not_none_ai_models = any(len(models) for models in all_models.values())
         if not not_none_ai_models:
             msg = "No models found"
             raise ValueError(msg)
-        log.debug(f"{not_none_ai_models=}")
         for key in all_models:
             if all_models[key]:
                 self._cache.set(key, all_models[key], CACHE_TTL, tag=Tag.AI_MODELS.value)
 
 
 def main():
     app = ChatApp()
```

### Comparing `paita-0.1.7/src/paita/tui/error_screen.py` & `paita-0.1.8/src/paita/tui/error_screen.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,8 +18,8 @@
         with VerticalScroll(id="error_screen_vertical"):
             yield Label(self._error, id="error_screen_label")
             with Horizontal(id="error_screen_button_block"):
                 yield Button(self._button_text, variant="primary", id="error_screen_button")
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "error_screen_button":
-            self.dismiss("ok")
+            self.dismiss(False)
```

### Comparing `paita-0.1.7/src/paita/tui/message_box.py` & `paita-0.1.8/src/paita/tui/message_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     def compose(self) -> ComposeResult:
         role_label = ROLE_ABBREVIATIONS[self._role]
         yield Label(role_label, classes=f"{self._role}_label")
         self._message_content = MessageContent(self.data, classes="markdown")
         yield self._message_content
 
     def on_mount(self) -> None:
-        self._update_timer = self.set_interval(1 / 2, self._markdown_update, pause=True)
+        self._update_timer = self.set_interval(1 / 4, self._markdown_update, pause=True)
 
     def append(self, data: str):
         self.data += data
         self._update_timer.resume()
 
     def flush(self):
         if self._update_timer:
```

### Comparing `paita-0.1.7/src/paita/tui/settings_screen.py` & `paita-0.1.8/src/paita/tui/settings_screen.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         settings: SettingsManager,
         cache: DiskCache,
         allow_cancel: bool = False,
     ):
         super().__init__()
         self._settings: SettingsManager = settings
         self._model: SettingsModel = settings.model.model_copy()
-        # log.debug(f"{self._model=}")
         self._cache: DiskCache = cache
         self._allow_cancel: bool = allow_cancel
 
         # Prefill select options based on stored settings values
         self._ai_services: List[Tuple[str, str]] = list(self._cache.keys(tag=Tag.AI_MODELS.value))
         if self._model.ai_service not in self._ai_services:
             self._model.ai_service = self._ai_services[0]
@@ -85,15 +84,15 @@
                 )
                 yield Input(
                     placeholder=label.AI_HISTORY_DEPTH,
                     value=to_str(self._model.ai_history_depth),
                     id="ai_history_depth",
                     classes="settings_input",
                     type="integer",
-                    validators=[Number(minimum=1, maximum=100)],
+                    validators=[Number(minimum=0, maximum=100)],
                     # max_length=2,
                 )
                 yield Input(
                     placeholder=label.AI_N,
                     value=to_str(self._model.ai_n),
                     id="ai_n",
                     classes="settings_input",
@@ -124,45 +123,44 @@
     async def on_mount(self) -> None:
         if self._model.ai_service is Select.BLANK or self._model.ai_model is Select.BLANK:
             self.query_one("#apply").disabled = True
 
     @on(Select.Changed)
     async def select_changed(self, event: Select.Changed) -> None:
         if event.control.id == "ai_service":
+            value = event.value
+            if value == self._model.ai_service:
+                return
             models = self._cache.get(event.value, Select.BLANK, tag=Tag.AI_MODELS.value)
             widget: Select = self.query_one("#ai_model")
             widget.set_options((item, item) for item in models)
         elif event.control.id == "ai_model":
+            value = event.value
+            if value == self._model.ai_model:
+                return
             self.query_one("#apply").disabled = False
         else:
             log.error(f"Undefined {event.id=}")
 
     async def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "apply":
             model: SettingsModel = SettingsModel(
                 ai_service=self.query_one("#ai_service").value,
                 ai_model=self.query_one("#ai_model").value,
-                # ai_persona=self.query_one("#ai_persona").text,
-                # ai_streaming=self.query_one("#ai_streaming").value,
-                # ai_model_kwargs=json.loads(self.query_one("#ai_model_kwargs").value),
-                # ai_n=self.query_one("#ai_n").value,
-                # ai_max_tokens=self.query_one("#ai_max_tokens").value,
-                # ai_history_depth=self.query_one("#ai_history_depth").value,
             )
             if (value := self.query_one("#ai_persona").text) != "":
                 model.ai_persona = value
             if (value := self.query_one("#ai_model_kwargs").value) != "":
                 model.ai_model_kwargs = str_to_dict(value)
             if (value := self.query_one("#ai_n").value) != "":
                 model.ai_n = str_to_num(value)
             if (value := self.query_one("#ai_max_tokens").value) != "":
                 model.ai_max_tokens = str_to_num(value)
             if (value := self.query_one("#ai_history_depth").value) != "":
                 model.ai_history_depth = str_to_num(value)
             model.ai_streaming = self.query_one("#ai_streaming").value
 
-            # log.debug(f"{model=}")
             self._settings.model = model
             await self._settings.save()
             self.dismiss(True)
         else:
             self.dismiss(False)
```

### Comparing `paita-0.1.7/src/paita/tui/wait_screen.py` & `paita-0.1.8/src/paita/tui/wait_screen.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/tui/styles/app.tcss` & `paita-0.1.8/src/paita/tui/styles/app.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/tui/styles/error_screen.tcss` & `paita-0.1.8/src/paita/tui/styles/error_screen.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/tui/styles/message_box.tcss` & `paita-0.1.8/src/paita/tui/styles/message_box.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/tui/styles/settings_screen.tcss` & `paita-0.1.8/src/paita/tui/styles/settings_screen.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/tui/styles/wait_screen.tcss` & `paita-0.1.8/src/paita/tui/styles/wait_screen.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/utils/settings_manager.py` & `paita-0.1.8/src/paita/utils/settings_manager.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/utils/settings_model.py` & `paita-0.1.8/src/paita/utils/settings_model.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/src/paita/utils/string_utils.py` & `paita-0.1.8/src/paita/utils/string_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 
 import json
 import re
 from typing import Any
 
 
 def to_str(value: Any) -> str | None:
-    return str(value) if value else None
-
-
-def from_str(value: str or None) -> Any | None:
-    return str(value) if str else ""
+    return str(value)
 
 
 def str_to_num(value: float | str) -> float | str:
     if isinstance(value, (float, int)):
         return value
     if isinstance(value, str):
         try:
```

### Comparing `paita-0.1.7/tests/integration/ai/test_chat.py` & `paita-0.1.8/tests/integration/ai/test_chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from paita.ai.chat import AsyncHandler, Chat
 from paita.ai.chat_history import ChatHistory
 from paita.ai.enums import AIService
 from paita.utils.settings_model import SettingsModel
 
 ai_service_models = {
     AIService.AWSBedRock.value: "anthropic.claude-v2",
-    # AIService.OpenAIChatGPT.value: "gpt-3.5-turbo",
+    AIService.OpenAI.value: "gpt-3.5-turbo",
+    AIService.Ollama.value: "openchat",
 }
 
 
 @pytest.fixture(params=list(ai_service_models.items()))
 def settings_model(request):
     key, value = request.param
     return SettingsModel(ai_service=key, ai_model=value)
@@ -39,39 +40,44 @@
 
 
 @pytest.fixture
 def chat_history():
     return ChatHistory(app_name="test", app_author="test", file_history=False)
 
 
-@pytest.mark.skip("Need to setup github action permissions")
 @pytest.mark.integration
 @pytest.mark.usefixtures("mock_env")
 def test_init_models(chat, settings_model, callback_handler):
     chat.init_model(
         settings_model=settings_model,
         callback_handler=callback_handler,
     )
 
 
-@pytest.mark.skip("Need to setup github action permissions")
 @pytest.mark.integration
 @pytest.mark.asyncio
 async def test_request_empty_history(chat, chat_history, settings_model, callback_handler):
+    if settings_model.ai_service == AIService.Ollama.value:
+        # Skip testing requests with ollama as it's too slow
+        return
+
     chat.init_model(
         settings_model=settings_model,
         callback_handler=callback_handler,
     )
 
     await chat.request("First", chat_history=chat_history)
 
 
-@pytest.mark.skip("Need to setup github action permissions")
 @pytest.mark.integration
 @pytest.mark.asyncio
 async def test_request_some_history(chat, chat_history, settings_model, callback_handler):
+    if settings_model.ai_service == AIService.Ollama.value:
+        # Skip testing requests with ollama as it's too slow
+        return
+
     chat.init_model(
         settings_model=settings_model,
         callback_handler=callback_handler,
     )
     await chat.request("First", chat_history=chat_history)
     await chat.request("Second", chat_history=chat_history)
```

### Comparing `paita-0.1.7/tests/unit/test_cache3.py` & `paita-0.1.8/tests/unit/test_cache3.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/tests/unit/test_settings_manager.py` & `paita-0.1.8/tests/unit/test_settings_manager.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/tests/unit/test_string_utils.py` & `paita-0.1.8/tests/unit/test_string_utils.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/tests/unit/ai/test_chat.py` & `paita-0.1.8/tests/unit/ai/test_chat.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/.gitignore` & `paita-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/LICENSE` & `paita-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paita-0.1.7/README.md` & `paita-0.1.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -48,11 +48,22 @@
 export OPENAI_API_KEY=<OpenAI API Key>
 ```
 
 #### AWS Bedrock
 
 Enable AI model access in AWS Bedrock. Configure aws credential access accordingly.
 
+#### Ollama
+
+Ollama enables running chat models locally. 
+
+Install [ollama](https://ollama.com) for operating system or use official (docker image)[https://hub.docker.com/r/ollama/ollama] 
+
+Once ollama installed pull desired model from a registry e.g.
+```
+ollama pull llama2
+```
+
 ## Feedback
 
 * [Issues](https://github.com/villekr/paita/issues)
 * [Discussion](https://github.com/villekr/paita/discussions)
```

### Comparing `paita-0.1.7/pyproject.toml` & `paita-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,25 +17,26 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "textual~=0.53",
+  "textual==0.54",  # 0.51 ok, 0.52 ok, 0.53 nok, 0.54 nok
   "boto3~=1.34",
   "loguru~=0.7",
   "langchain~=0.1",
   "langchain-openai~=0.1",
   "appdirs~=1.4",
   "pydantic~=2.6",
   "cache3~=0.4",
   "aiofiles~=23.2",
   "pyperclip~=1.8",
-  "eval-type-backport~=0.1"
+  "eval-type-backport~=0.1",
+  "aiohttp~=3.9.3",
 ]
 
 [project.urls]
 Documentation = "https://github.com/villekr/paita#readme"
 Issues = "https://github.com/villekr/paita/issues"
 Source = "https://github.com/villekr/paita"
 
@@ -62,22 +63,27 @@
   "appdirs-stubs",
   "types-aiofiles"
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
+github-test-cov = 'coverage run -m pytest -m "not integration" {args:tests}'
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
+github-cov = [
+  "github-test-cov",
+  "cov-report",
+]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
```

### Comparing `paita-0.1.7/PKG-INFO` & `paita-0.1.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: paita
-Version: 0.1.7
+Version: 0.1.8
 Summary: paita - Python AI Textual Assistant
 Project-URL: Documentation, https://github.com/villekr/paita#readme
 Project-URL: Issues, https://github.com/villekr/paita/issues
 Project-URL: Source, https://github.com/villekr/paita
 Author-email: Ville Kärkkäinen <ville.karkkainen@outlook.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -16,24 +16,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: aiofiles~=23.2
+Requires-Dist: aiohttp~=3.9.3
 Requires-Dist: appdirs~=1.4
 Requires-Dist: boto3~=1.34
 Requires-Dist: cache3~=0.4
 Requires-Dist: eval-type-backport~=0.1
 Requires-Dist: langchain-openai~=0.1
 Requires-Dist: langchain~=0.1
 Requires-Dist: loguru~=0.7
 Requires-Dist: pydantic~=2.6
 Requires-Dist: pyperclip~=1.8
-Requires-Dist: textual~=0.53
+Requires-Dist: textual==0.54
 Description-Content-Type: text/markdown
 
 # Paita - Python AI Textual Assistant
 <img src="https://github.com/villekr/paita/blob/main/imgs/paita.jpg?raw=true" width="800">
 
 Paita is textual assistant for your terminal that supports multiple AI Services and models.
 
@@ -82,11 +83,22 @@
 export OPENAI_API_KEY=<OpenAI API Key>
 ```
 
 #### AWS Bedrock
 
 Enable AI model access in AWS Bedrock. Configure aws credential access accordingly.
 
+#### Ollama
+
+Ollama enables running chat models locally. 
+
+Install [ollama](https://ollama.com) for operating system or use official (docker image)[https://hub.docker.com/r/ollama/ollama] 
+
+Once ollama installed pull desired model from a registry e.g.
+```
+ollama pull llama2
+```
+
 ## Feedback
 
 * [Issues](https://github.com/villekr/paita/issues)
 * [Discussion](https://github.com/villekr/paita/discussions)
```

