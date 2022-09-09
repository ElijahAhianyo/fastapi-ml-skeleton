# Fastapi Skeleton Main

[_Documentation generated by Documatic_](https://www.documatic.com)

<!---Documatic-section-Codebase Structure-start--->
## Codebase Structure

<!---Documatic-block-system_architecture-start--->
```mermaid
None
```
<!---Documatic-block-system_architecture-end--->

# #
<!---Documatic-section-Codebase Structure-end--->

<!---Documatic-section-fastapi_skeleton.main.get_app-start--->
## fastapi_skeleton.main.get_app

<!---Documatic-section-get_app-start--->
<!---Documatic-block-fastapi_skeleton.main.get_app-start--->
<details>
	<summary><code>fastapi_skeleton.main.get_app</code> code snippet</summary>

```python
def get_app() -> FastAPI:
    fast_app = FastAPI(title=APP_NAME, version=APP_VERSION, debug=IS_DEBUG)
    fast_app.include_router(api_router, prefix=API_PREFIX)
    fast_app.add_event_handler('startup', start_app_handler(fast_app))
    fast_app.add_event_handler('shutdown', stop_app_handler(fast_app))
    return fast_app
```
</details>
<!---Documatic-block-fastapi_skeleton.main.get_app-end--->
<!---Documatic-section-get_app-end--->

# #
<!---Documatic-section-fastapi_skeleton.main.get_app-end--->

[_Documentation generated by Documatic_](https://www.documatic.com)