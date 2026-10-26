import httpx
import pandas as pd

def testar_ambiente():
    print("Iniciando testes do ambiente virtual...\n")
    
    # 1. Testando Bibliotecas de Coleta (HTTPX)
    url = "https://practicesoftwaretesting.com/"
    try:
        response = httpx.get(url)
        if response.status_code == 200:
            print("✅ Coleta: Ambiente configurado com sucesso! Conexão HTTPX ativa.")
        else:
            print(f"⚠️ Coleta: Conexão estabelecida, mas o status retornado foi: {response.status_code}")
    except Exception as e:
        print(f"❌ Coleta: Falha ao tentar conectar na rede: {e}")

    # 2. Testando Bibliotecas de Análise (Pandas)
    try:
        versao = pd.__version__
        print(f"✅ Análise: Pandas importado com sucesso! Versão instalada: {versao}")
    except Exception as e:
        print(f"❌ Análise: Erro ao importar o Pandas: {e}")

if __name__ == "__main__":
    testar_ambiente()