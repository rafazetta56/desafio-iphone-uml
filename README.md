@startuml

class iPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {
  + tocar()
  + pausar()
  + selecionarMusica(musica: String)
  + ligar(numero: String)
  + atender()
  + iniciarCorreioVoz()
  + exibirPagina(url: String)
  + adicionarNovaAba()
  + atualizarPagina()
}
interface ReprodutorMusical {
  {abstract} + tocar()
  {abstract} + pausar()
  {abstract} + selecionarMusica(musica: String)
}

interface AparelhoTelefonico {
  {abstract} + ligar(numero: String)
  {abstract} + atender()
  {abstract} + iniciarCorreioVoz()
}

interface NavegadorInternet {
  {abstract} + exibirPagina(url: String)
  {abstract} + adicionarNovaAba()
  {abstract} + atualizarPagina()
}

@enduml
