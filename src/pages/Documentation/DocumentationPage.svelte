<script>
  import Table from "../../components/Table/Table.svelte";
  import ReportsTableItem from "./components/DocumentationTable/ReportsTableItem.svelte";
  import WebsiteTableItem from "./components/DocumentationTable/WebsiteTableItem.svelte";
</script>

<section class="text-gray-700 body-font">
  <div class="container px-5 py-24 mx-auto">
    <div class="flex flex-col text-center w-full mb-20">
      <h1 class="title-section">Documentation</h1>
      <p class="subtitle-section lg:w-2/3 mx-auto">
        We decided to make the whole company process open-source, so that
        everyone can learn with our process and make their own thing.
      </p>
    </div>
    <div class="lg:w-2/3 w-full mx-auto overflow-auto mb-12">
      <Table headers={["Document", "Iteration"]} title="Reports">
        <ReportsTableItem
          version="v1.1"
          link="/assets/e2.pdf"
          name="E2: Relatório Técnico: Visão do Projeto"
        />
        <ReportsTableItem
          version="v1.1"
          link="/assets/e3.pdf"
          name="E3: Relatório Técnico: Análise"
        />
        <ReportsTableItem
          version="v1.1"
          link="/assets/e4.pdf"
          name="E4: Relatório Técnico: Protótipo"
        />
      </Table>
    </div>
    <div class="lg:w-2/3 w-full mx-auto overflow-auto mb-12">
      <Table headers={["Version", "Date", "Author", "Changes"]} title="Website">
        <WebsiteTableItem
          version="v1.0"
          date="11/10/2020"
          author="Vasco Sousa"
          changes="Initial layout, pages and images."
        />
        <WebsiteTableItem
          version="v1.1"
          date="16/01/2021"
          author="Vasco Sousa"
          changes="Add application links and reports."
        />
      </Table>
    </div>
  </div>
</section>
