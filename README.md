# remove_rails_delayed_job
Passo a passo de como remover a gema depois de instalada e configurada.

1 - Fazer o rollback da migration, ex.: 'rails db:rollback STEP=1';

2 - Tirar a gema do Gemfile;

3 - Deletar migration da criação tabela delayed_jobs;

4 - Tirar a configuração do DelayedJob no arquivo application_controller.rb;

5 - Deletar arquivo de configuração da DelayedJob chamado delayed_job_config.rb;

6 - Apagar a tabela delayed_jobs, ex.: ActiveRecord::Migration.drop_table(:delayed_jobs);


