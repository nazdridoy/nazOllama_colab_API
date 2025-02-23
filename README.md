# nazOllama Colab API 🦙

Run Ollama models on Google Colab's free T4 GPU and expose a compatible API endpoint accessible from anywhere!

## 🌟 Features

- Run Ollama on Google Colab's free GPU (T4)
- OpenAI-compatible API endpoint via Cloudflare Tunnel
- Support for multiple Ollama models
- Persistent URL storage via Filebin
- Easy-to-use Jupyter notebook interface

## 🚀 Quick Start

1. Open the notebook in Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nazdridoy/nazOllama_colab_API/blob/main/nazOllama_colab_API.ipynb)

2. Run the blocks in order:
   - Check GPU availability
   - Install Ollama and Cloudflare Tunnel
   - Start Ollama server
   - Pull your desired model
   - List available models
   - Expose the API via Cloudflare Tunnel

## 📚 Supported Models

- deepseek-r1
- llama3.2
- qwen2.5
- mistral
- qwen2.5-coder
- mixtral
- *Any other Ollama-compatible model*

## 🔧 API Usage

Once the API is exposed, you can use it like this:
```
curl -X POST http://<your-api-url>/api/generate \
  -H "Content-Type: application/json" \
  -d '{"model":"llama3.2:3b","prompt":"Hello, how are you?"}'
```

## ⚠️ Important Notes

- The Colab session will disconnect after 90 minutes of inactivity
- GPU runtime is limited to 3-12 hours per session ( Resources offered free of charge are not guaranteed.)
- Use responsibly and in accordance with Google Colab's terms of service

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Ollama](https://ollama.ai/) for the amazing model serving framework
- [Cloudflare](https://www.cloudflare.com/) for the tunnel service
- [Google Colab](https://colab.research.google.com) for providing free GPU access

## 👤 Author

- [@nazdridoy](https://github.com/nazdridoy)