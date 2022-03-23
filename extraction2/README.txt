09/03/22


pour le moment, les données ne sont pas du tout nettoyées.

Il y a 32 colonnes
COLUMNS :

'public_identifier', 				id du profil linkedin souvent sous le format prénom-nom-8ou9intET/OUchar ou chaine
 'profile_pic_url',				lien de la photo de profil (on y a jamais accès, pas exploitable) 
 'background_cover_image_url',		lien image de couverture (on y a jamais accès, pas exploitable)
 'first_name',					prénom
 'last_name',					nom
 'full_name',					prénom nom
 'occupation',					profession
 'headline',					titre professionnel
 'summary',						phrase d'accroche (présentation, description)
 'country',						code pays en 2 lettres 
 'country_full_name',				nom complet du pays
 'city',						nom complet de la ville
 'state',						nom complet de l'état
 
'experiences',					liste des expériences composée de une ou plusieurs expériences chacune composée de
							[starts_at, ends_at, company, company_linkedin_profile_url, title, description, location, logo_url (lien non exploitable)]
							les champs "starts_at" et "ends_at" sont composés de [day, month, year]
 
'education',					liste des formations composée de une ou plusieurs formation chacune composée de
							[starts_at, ends_at, field_of_study, degree_name, school, description (de la formation), logo_url (lien non exploitable)
							les champs "starts_at" et "ends_at" sont composés de [day, month, year]
 
'languages',					liste des langues
 
'accomplishment_organisations',		liste des prix composée de [starts_at, ends_at, org_name, title, description]
							les champs "starts_at" et "ends_at" sont composés de [day, month, year]
 
'accomplishment_publications',		liste des prix composée de [title, issuer (organisme qui donne le prix), issued_on (date à laquelle le prix a été émis), description]
							le champs "issued_on" est composé de [day, month, year]
 
'accomplishment_honors_awards',		starts_at, ends_at, cause, company, company_linkedin_profile_url, title, description, logo_url
 
'accomplishment_patents',			prix concernant les soft skils et qualités morales de la personne
							[name ou title]
 
'accomplishment_courses',			
							["name", "link"/"url", "summary"/"description", "location", "starts_at", "ends_at", ]
 
'accomplishment_projects',			[starts_at", "ends_at", "url", "name", "license_number", "display_source", "authority", "summary", "location"]
 
'accomplishment_test_scores',
							["starts_at", "ends_at", "cause", "company", "company_linkedin_profile_url", "title", "description", "logo_url"]
							

 'volunteer_work',				listes des actions bénévoles
							["link", "name", "summary", "location"]

 'certifications',				liste des certifications publiées ou liké
							publié ["starts_at", "ends_at", "url", "name", "license_number","display_source", "authority"]
							liké ["title", "activity_status"]

 'connections',					nombre de relations
 'people_also_viewed',				liste contenant des liens vers des profils ayant également été consultés par ceux qui ont consulté ce profil
 'recommendations',				liste des recommendations
 
'activities',					liste des activités publiés ou liké par la personne
							publié ["name", "link", "summary", "location"]
							liké ["title", "link", "activity_status"]
 
'similarly_named_profiles',			liste contenant des liens vers des profils de personnes ayant le même nom et prénom

 'articles',					liste des articles publiés par la personne
							["title", "author", "published_date", "image_url"]

 'groups'						cette information est disponible pour seulement 2 des 4 fichiers, à savoir : united_states_profiles.txt et singapore_profiles.txt
							liste composée de [profile_pic_url (lien image profil du groupe non exploitable), name (nom du groupe), url (lien du groupe)



liste des colonnes atomiques : [ 'public_identifier','profile_pic_url','background_cover_image_url','first_name','last_name','full_name','occupation','headline','summary','country',
 'country_full_name','city','state', 'connections']

informations complémentaires :
les champs "starts_at", "ends_at" et "issued_on" sont composés de [day, month, year]
les liens 'profile_pic_url', 'background_cover_image_url' et "logo_url" ne sont pas exploitable