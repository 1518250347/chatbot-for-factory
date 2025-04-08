# DeepSeek 智能助手

这是一个通过OLLAMA调用DeepSeek本地大模型接口的AI对话系统，具有网页界面和知识库管理功能。

## 功能特点

- 基于OLLAMA调用本地DeepSeek模型
- 实时网页对话界面
- 知识库管理（添加、删除、查询）
- 基于知识库内容的专业问答

## 系统要求

- Python 3.7+
- OLLAMA服务已安装并运行
- DeepSeek模型已在OLLAMA中下载

## 安装步骤

1. 克隆或下载本项目

2. 安装依赖包
   ```
   pip install -r requirements.txt
   ```

3. 确保OLLAMA服务已启动并加载DeepSeek模型
   ```
   # 如果尚未下载DeepSeek模型，请先运行
   ollama pull deepseek
   
   # 启动OLLAMA服务
   ollama serve
   ```

4. 启动应用
   ```
   python app.py
   ```

5. 在浏览器中访问 http://localhost:5000

## 使用说明

### 对话功能

- 在主界面的输入框中输入问题，点击发送按钮或按Enter键发送
- 系统会自动从知识库中检索相关信息，并结合DeepSeek模型的能力回答问题

### 知识库管理

- 点击左侧边栏