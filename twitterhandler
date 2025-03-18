from smolagents import CodeAgent, Tool
from jinja2 import Template
class TwitterFormatterTool(Tool):
    def __init__(self):
        super().__init__(name="TwitterFormatter", description="Format text for Twitter.")

    def __call__(self, text):
        # Ensure text fits within Twitter's character limit (280 characters)
        if len(text) > 280:
            return text[:277] + "..."
        return text
