本项目利用spring-ai-alibaba-graph实现深度研究

### 工具
- tavily API文档：https://docs.tavily.com/documentation/api-reference/endpoint/search
- 高德地图MCP：https://lbs.amap.com/api/mcp-server/gettingstarted#t1

macos:

mcp-servers.json

```json
{
  "mcpServers": {
    "amap-maps": {
      "command": "npx",
      "args": ["-y", "@amap/amap-maps-mcp-server"],
      "env": {
        "AMAP_MAPS_API_KEY": "AMAP_MAPS_API_KEY"
      }
    }
  }
}
```

windows:

mcp-servers-windows.json

记得删掉`-windows`，命名和macos的一致，只需要保留一个文件即可

```json
{
  "mcpServers": {
    "amap-maps": {
      "command": "cmd",
      "args": ["/c","npx","-y","@amap/amap-maps-mcp-server"],
      "env": {
        "AMAP_MAPS_API_KEY": "AMAP_MAPS_API_KEY"
      }
    }
  }
}
```



### 主要参与贡献
GitHub: 
- yingzi： 整体架构设计，流程实现
- zhouyou0527：ResearcherNode、CoderNode实现
